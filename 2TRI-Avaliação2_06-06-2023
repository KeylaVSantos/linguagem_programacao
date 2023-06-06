import PySimpleGUI as sg

sg.theme('DefaultNoMoreNagging')

layout = [ 
            [sg.Text("CALCULADOR DE IMC")],
            [sg.Text("Massa: "),sg.Input(key="-MASS-",size=(30))],
            [sg.Text("Altura: "),sg.Input(key="-HEIGHT-",size=(30))],
            [sg.Push(),sg.Button("Calcular"),sg.Push()]
         ]

window = sg.Window("IMC",layout=layout,font="Monaco 20",element_justification="center")

while True:
    event, value = window.read()
    print(event, value)
    Massa=float(value["-MASS-"])
    Altura=float(value["-HEIGHT-"])
    IMC = Massa / (Altura**2)
    sg.Popup(f"Seu IMC é {IMC:.2F}", font="26")
    if event == "QUIT" or event == sg.WIN_CLOSED:
      break

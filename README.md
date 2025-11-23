import time
import pyautogui
import keyboard

def abrir_navegador_e_youtube():
    time.sleep(0.5)
    #abrir o navegador
    pyautogui.press('win')
    time.sleep(0.5)
    pyautogui.write('google Chrome')
    pyautogui.press('enter')
    time.sleep(1.5)
    #abrir o youtube
    pyautogui.click(x=1084, y=468)  # Coordenadas da barra de endereços
    pyautogui.write('youtube.com')
    pyautogui.press('enter')
keyboard.add_hotkey('ctrl+alt+s', abrir_navegador_e_youtube)
keyboard.wait('esc')

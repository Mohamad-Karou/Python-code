import tkinter


class TempConverterGUI:

    def __init__(self):
        # create main window
        self.mw = tkinter.Tk()
        # set the title of the main window
        self.mw.title("Temperature Converter")

        # Create three frames in the main window, that will group different widgets
        self.top_frame = tkinter.Frame(self.mw)
        self.mid_frame = tkinter.Frame(self.mw)
        self.bottom_frame = tkinter.Frame(self.mw)

        # Create the widgets for the top frame
        self.prompt_label = tkinter.Label(self.top_frame, text="Enter Temperature in Celsius")
        self.temp_entry = tkinter.Entry(self.top_frame, width=15)

        # Pack the widgets in the top frame
        self.prompt_label.pack(side="left")
        self.temp_entry.pack(side="left")

        # Create widgets for mid frame
        self.desc_label = tkinter.Label(self.mid_frame, text="Converted Temperature in Fahrenheit : ")
        # Create a StringVar object that will store the converted temperature
        self.result = tkinter.StringVar()
        # Create a label that will be used to display the result
        self.result_label = tkinter.Label(self.mid_frame, textvariable=self.result)

        # Pack the widgets for mid-frame
        self.desc_label.pack(side="left")
        self.result_label.pack(side="left")

        # Create widgets for the bottom frame
        self.calc_button = tkinter.Button(self.bottom_frame, text="Convert", command=self.convert)
        self.quit_button = tkinter.Button(self.bottom_frame, text="Quit", command=self.mw.destroy)

        # Pack the buttons for bottom window
        self.calc_button.pack(side="left")
        self.quit_button.pack(side="left")

        # Pack the frames
        self.top_frame.pack()
        self.mid_frame.pack()
        self.bottom_frame.pack()

        # Enter tkinter mainloop
        tkinter.mainloop()

    def convert(self):
        # Get the celsius value
        celsius = float(self.temp_entry.get())
        # Convert celsius into fahrenheit
        fahrenheit = (9 / 5) * celsius + 32
        self.result.set(str(fahrenheit))


# Create an instance of Temp_Converter_GUI
gui = TempConverterGUI()

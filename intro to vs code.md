Hello everyone, I am Abdul Baseer studying in final year. I have created the following repository for different combinational and sequential circuits. This is about introduction to vs code

1.MUX(Combinational Circuit)

Steps:

![image](https://user-images.githubusercontent.com/93662214/140520203-e13677a6-6c17-4f26-98bb-19f06223e630.png)

Click on the mark icon, Then make a new folder by naming it.

Again beside the mark icon click on it, follow the same procedure to make new subfolders.

![image](https://user-images.githubusercontent.com/93662214/140520674-427470cf-8cbd-4bae-98fe-896d28a23476.png)

Write the verilog program in the blank field and Save it by pressing Ctrl+s.

![image](https://user-images.githubusercontent.com/93662214/140520955-2e26cf7e-47f4-4829-9185-2c44468a9350.png)

Go to another sub-folder and write the testbench for the above verilog program written.

![image](https://user-images.githubusercontent.com/93662214/140521355-cded84d3-6a4c-4bbd-9b23-7aeae4de0403.png)

Write the shown command, to be in working file. Command syntax={cd tabfoldername.v}

![image](https://user-images.githubusercontent.com/93662214/140521594-daf38429-a58c-4265-a8df-0d12d3a113b0.png)

command written is for to check sub-folders

![image](https://user-images.githubusercontent.com/93662214/140521843-de4cb042-9c2b-4749-96ad-cea5d869e014.png)

Further, to check for the codes to be error free use the shown command. By successful error free codes, a file gets generated as (a.out).

command syntax={iverilog tabverilogcodesubfoldername.v tabtestbenchsubfolder.v}

![image](https://user-images.githubusercontent.com/93662214/140522569-820f25a2-5369-47e1-9b76-37cf99177c03.png)

To run the simulation, have the following command

command syntax={vvp taba}

A new file will be generated with the processing foldername.vcd

![image](https://user-images.githubusercontent.com/93662214/140523063-f85c75f4-175d-4dee-9e18-aec9a5cb76a3.png)

Now to generate the waveform Enter the command (gtkwave tabprocessingfoldername.vcd).

![image](https://user-images.githubusercontent.com/93662214/140523367-cfb75a8c-1ff0-469a-862b-f64f3d3e7693.png)

Attach the cmos (program) lib file or liberty file in the processing folder.

![image](https://user-images.githubusercontent.com/93662214/140523624-554f76ad-8aa9-426e-b305-92382b51ed71.png)

Now go to yosys by giving the command {yosys}

![image](https://user-images.githubusercontent.com/93662214/140524140-31f47d7e-8144-40e2-9ff0-9c30c9f60ace.png)

To read the liberty file, Enter the command shown in demonstration image.

![image](https://user-images.githubusercontent.com/93662214/140524442-bb65d53c-1eed-4372-b083-9216ebfe0491.png)

For executing verilog frontend. Enter read_verilog(processingfilename.v).

![image](https://user-images.githubusercontent.com/93662214/140524732-dc9ddae9-10da-4451-96e8-a15d517378a7.png)

To synthesize, Enter synth -top modulename

![image](https://user-images.githubusercontent.com/93662214/140524982-f67211a4-49f6-4033-8976-eb0f7985ad5f.png)

To execute, Enter the shown command in demonstration image.

![image](https://user-images.githubusercontent.com/93662214/140525238-81761924-6f2d-4b9e-a4fc-186f1da2b3b5.png)

To generate the show.dot file, Enter the command(show modulename).

![image](https://user-images.githubusercontent.com/93662214/140525964-1f4ade21-a951-4a43-905d-abc5fbf534b9.png)

After the successful generation of show.dot file

Then click on show.dot file

Go to view from the following list in view select(command palette) or PRESS ctrl+shift+P. Further enter or select Graphviz:- open preview to the slide

![image](https://user-images.githubusercontent.com/93662214/140529296-c54dd9cd-e0e7-43dd-b23e-f17b0a705428.png)

Finally, Successful generation of output or preview to the slide

Up down counter(Sequential Circuit)

In this synthesis process we are using SKY 130 library file. ll the required files will be provided above. After downloading all the required files you will see the folder like this

![image](https://user-images.githubusercontent.com/93662214/140532658-edd87178-ab8a-4dad-838e-8d8a45aae32e.png)

open that highlighted folder in which you willfind another two more folders open simultaneously these two folders and copy all the files from it the beginning.(total 3 files you have to copy and paste names are as follows).

![image](https://user-images.githubusercontent.com/93662214/140533134-ad24baea-606a-4edb-844b-dd70cf648937.png)

1. sky130_fd_sc_hd__tt_025C_1v80.lib
2. sky130_fd_sc_hd.v
3. primitives.v

![image](https://user-images.githubusercontent.com/93662214/140533638-149d2274-2686-4b6b-af45-f166ee24dc30.png)

now come back to the VScode Terminal and follow the below given steps for simulation.

Step1:- In terminal type yosys to open yosys tool

![image](https://user-images.githubusercontent.com/93662214/140534263-e8faa6d9-6c21-4339-a439-644371c50e81.png)

Step 2:- If no errors come then follow the next command type: read_liberty -lib sky 130_fd_sc_hd__tt_025C-1v80.lib

![image](https://user-images.githubusercontent.com/93662214/140536561-bf922de2-b811-426f-8ec3-21a6db31f8f5.png)

Step 3:- after that type read_verilog filename.v // this command is use for reading module written in verilog

![image](https://user-images.githubusercontent.com/93662214/140536871-cef890d8-a5d1-43b3-866a-4f51193e5f99.png)

Step 4:- After that use syntax for synthesis process: synth -top modulename.

![image](https://user-images.githubusercontent.com/93662214/140537436-0f55ed21-356d-411f-b067-ac2b51e56d96.png)

Step 5:- For mapping flip-flops to library use following command: dfflibmap-liberty sky130_fd_sc_hd__tt_025C_1v80.lib

![image](https://user-images.githubusercontent.com/93662214/140537770-b4f41fd6-a4b5-41fd-8c3c-c8411c6e12cc.png)

Step 6:- For mapping logic to library file use following command: abc-liberty sky130_fd_sc_hd__tt_025C_1v80.lib

![image](https://user-images.githubusercontent.com/93662214/140538048-07358ddd-273c-4e06-8c69-43ec4c46cc53.png)

Step 7:- For downloading netlist file type: show

![image](https://user-images.githubusercontent.com/93662214/140538375-5b221824-abf0-4b0f-b5d5-92745182c6b0.png)

![image](https://user-images.githubusercontent.com/93662214/140538669-d6253160-fc3d-4876-97fe-ade5b5714683.png)

Step 8:- Now use following command: tee -o report.txt stat -liberty sky_130_fd_sc_hd__tt_025C_1v80.lib

![image](https://user-images.githubusercontent.com/93662214/140539177-2256d2dd-246a-4d6a-9dea-feee2023bc2c.png)

Step 9:- We are done with the synthesis now we need to download or write the synthesis file into some sort of file mainly in verilog format for this use: write_verilog -noattr netlist.v

![image](https://user-images.githubusercontent.com/93662214/140539531-740cd806-80c3-4755-bbbc-35520456e519.png)

Step 10:- Now we can exit for yosys tool for that simply type "exit" and hit enter

![image](https://user-images.githubusercontent.com/93662214/140539837-da309e53-16ff-4197-9169-1ab115c2380e.png)
at the end you will report.txt file and netlist.v

in which report.txt file shows the statisitical data of design made

![image](https://user-images.githubusercontent.com/93662214/140540077-e32b6554-c2fe-4cae-b6b9-2ac1f0df5281.png)
and netlist.v file shows all the detailed information which is required to make an integrated circuit. Ths is the file we gave to foundry for making a physical copy.

![image](https://user-images.githubusercontent.com/93662214/140540385-73b5cd28-e9ff-46b2-9731-1ab7a1f72278.png)

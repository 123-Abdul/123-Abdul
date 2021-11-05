Hi, myself Syed Abdul Baseer pirsuing my final year project. For being tenacious towards my final year project. I started working out to know the tools, by a few basic programs which are below following.

this is about intro to vs code

for using vs code

1.MUX

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

##Initial configuration 

You need to tell GIT who you are, this information is then automatically included in you commits. Run the following commands in your terminal:


```bash
git config --global user.name "John Doe"  
git config --global user.email johndoe@example.com  

```
>> **TIP:** to run a command in terminal type in the instructions and after each line press enter

**Optional Text Editor**

We can also tell git to use a  specific text editor, run the command below which instructs GIT to use Notepad++:

```bash
git config --global core.editor "'C:/Program Files (x86)/Notepad++/notepad++.exe' -multiInst -nosession"
```


**You can check your configuration with:**

```git config --list```



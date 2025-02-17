# In Class Problem Set 3

I used ComboBoxDemo.java a few years ago.  It used to compile cleanly.  Even though the code has not changed, it now  will not compile without throwing warnings.

Doing everything from a command prompt or Git Bash (no IDEs allowed), your mission is to debug the code and find out why it stopped compiling cleanly.  When you have figured it out,  note what you changed and why it stopped working in the README.md file.

##Riley Pierson and Alejandro Perez Jorda
##2/17/2025

**Changes to code**

21: static JComboBox cBox1 changed to static JComboBox<String> cBox1;

43: cBox1 = new JComboBox(s1) changed to cBox1 = new JComboBox<String>(s1);

**What caused it to stop working?**
JcomboBox was initialized with the generic data-type <E> (as default), therfore, it gave us a warning since we were using <Strings>

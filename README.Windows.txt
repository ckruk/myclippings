
Windows users have to customize the system and the script to the work:

1. Install Perl in the system (see: http://www.perl.org/get.html).

2. Rename myclippings script to myclippings.pl one.

3. Set $system variable in the script to "Windows" value.

4. Users of non-English versions of Windows should change $path variable
   from:

      $path = "$ENV{USERPROFILE}\\My Documents\\";

   to:

      $path = "$ENV{USERPROFILE}\\Moje dokumenty\\";

   or another value according to the name of "My Documents" directory.

The script in Windows version reads "My Clippings.txt" file from $path
directory and stores restored "My Clippings.txt" file in the same directory. 
In order to read and write "My Clippings.txt" file from and to the current
directory it is enough to set $path variable to an empty value.

In order to read the other documents provided with myclippings script as
well as in order to edit myclippings script Windows users should use WordPad
instead of Notepad because the latter can not inperpret properly LF line
endings.


This is a sample program that I wrote to learn more about using dialog  
boxes. It is not a perfect program but is useful . I have include the 'C'
source so other people can make modifications to better suit there needs.
   If anyone has suggestions on how to improve this program please let me
know. I can be reached on my BBS. Following is the info on it:

				      Compu-Plane
				      818 843-3507  300/1200/2400
				      818 843-4874  300/1200/2400/9600 on a Courier HST.
Both lines are 8,N,1 and are available 24 hrs a day. The BBS is also running 
in the protected mode of OS/2.

   There are two main menu selections. The first allows you to select the 
search parameters. The current drive is the default. This dialog box uses four can 
different styes of dialog entries(Listbox,Edit box,checkbox, and Pushbotton).
The second selection is the exit selection. It seems to make most users more
comfortable to have this selection, even though you can close it with the
system menu.

   Hopefully this example will help others develop OS/2 PM applications. You 
are free to pass this program along to others.


===========================================================================

                               
                                                   Corrections For OS/2 ver 1.2
                                                   ----------------------------------------------

	OS/2 ver 1.2 released in 1989 introduced the High Performance File System (HPFS)
which is a radical departure from the FAT file system used by DOS and CP/M.

	One of the innovations of the HPFS is the use of longer file names, and the
characters which may make up a file name.  The convention is much like Unix, except that
forward slashes (/) are not used as delimiters:  the HPFS still uses the DOS backslash 
(\ ).  

	Thus, under the HPFS, the following is a legal filename:

			this.test.file.for.program-a

	The complete pathname could be:

			d:\myfiles\this.test.file.for.program-a

	Naturally, this new naming convention presents a problem with OS/2 ver 1.0 and
1.1 file finding utilities, because the length of permissable filenames was usually hardcoded
in the program.  It was even hardcoded in the Microsoft header files.  Thus, these utilities 
would not work for the HPFS.

	AW.EXE is a nice program.  The coding is very well done.  With a few simple changes
I was able to port it to OS/2 ver 1.2.  I changed the necessary buffer sizes, and it now functions
under ver 1.2, and will locate files using the new naming conventions.

	The only other changes I made were in the appearance of the Dialog Box, and a 
cosmetic change to the strings emited after the search ( they needed a newline character added
so that they would wrap correctly ). 

	If these changes meet with your approval, your are free to use this uploaded
executable as you like.

				
						Harve Jay Schiffman

						CIS 72261,347

	


# activate_dos2unix

This little sh file fixes the problem when bash (cygwin) is trying to activate a venv created in a windows format. The windows 'activate' file (located in the directory 'Scripts') is incompatible with bash. 
The sh file searches for "Scripts/activate" files. It will make a copy of the 'activate' file, rename the copy to 'activateCyg' and then, 
using the bash method dos2unix this 'activateCyg' file will become compatible with bash and can be used to activate the venv.



DLL Injection
=============

Sample codes (Refined) to do DLL injection into a running process.
Added function hooking code to overwrite functions in WinSock.dll 
i.e send() ,recv()


How to compile:
	Under MSVC++
	Create a simple console project myinject.exe, which is a console application. Compile myinject.cpp into an executable. 

	Create another simple DLL project for mydll.dll. Compile mydll.dll into a DLL.


How to run:
	First run the executable which uses winsock( ws2_32.dll in particular) you want to inject, eg: mirc.exe

	Run myinject.exe with the following arguments:

		myinject.exe <Process Name to inject> <DLL path to inject>

	example:
		myinject.exe mirc.exe C:\tensaix2j\mydll.dll



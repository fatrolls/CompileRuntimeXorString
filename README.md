# CompileRuntimeXorString
Compile Encrypted Xor Strings in Run-Time only! Protect against crackers/hackers/anti-cheats, Support for char and wchar_t

Example code

	char test[5] = { 0 };
	strcpy(test, XorStr("blah"));
	printf("test = %s\n", test);
	wchar_t testw[5] = { 0 };
	wcscpy(testw, XorStrW(L"blah"));
	printf("test = %ls\n", testw);

	char buffertest[100];
	sprintf(buffertest, XorStr("hidden blah! %d"), 1234);
	printf(XorStr("value = %s\n"), buffertest);

	wchar_t buffertest2[100];
	swprintf(buffertest2, XorStrW(L"hahaha blah! %d"), 54321);
	printf(XorStr("value = %ls\n"), buffertest2);


Outputs

	test = blah
	test = blah
	value = hidden blah! 1234
	value = hahaha blah! 54321

Disassembly

![disasm1](https://github.com/fatrolls/CompileRuntimeXorString/screenshots/1.png)<br>
![disasm2](https://github.com/fatrolls/CompileRuntimeXorString/screenshots/2.png)<br>
![disasm3](https://github.com/fatrolls/CompileRuntimeXorString/screenshots/3.png)<br>

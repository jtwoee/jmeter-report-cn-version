For apache Jmeter version 5.1.1

	1. Download the report-template from github
	2. Replace the one under $JMETER_HOME/bin/report-template
	jmeter -g <log file> -o <Path to output folder>
	
	eg： jmeter -g c:/dev/jmeter/testReports.csv -o c:/dev/jmeter/target
	
You need to generate the report csv log file firstly

In case of Chinese charset issue, please modify your jmeter.bat file:

%JM_START% "%JM_LAUNCH%" -Dfile.encoding=utf-8 %ARGS% %JVM_ARGS% -jar "%JMETER_BIN%ApacheJMeter.jar" %JMETER_CMD_LINE_ARGS%

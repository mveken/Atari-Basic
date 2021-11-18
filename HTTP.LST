0 DIM A$(128)
1 POKE 766,1
10 OPEN #1,12,2,"N:HTTP://www.veken.nl":REM HTTP GET
20 XIO 77,#1,12,3,"N:":REM SET HEADERS
30 PRINT #1;"Authorization: Basic dGhvbWM6ZTF4YjY0WEM0Ng=="
31 XIO 77,#1,12,1,"N:":REM COLLECT HEADERS
32 ? #1;"Date":? #1;"Content-Length"
33 XIO 77,#1,12,2,"N:":REM GET HEADERS
34 ? :? "Headers:":? 
35 ? "Date: ";:INPUT #1,A$:? A$
36 ? "Content-Length: ";:INPUT #1,A$:? A$
37 ? :? 
40 XIO 77,#1,12,0,"N:":REM GET BODY
50 TRAP 70
60 INPUT #1,A$:? A$:GOTO 60
70 CLOSE #1:POKE 766,0:END 

BEGIN   % A TEST OF PROCDEURES AND RECURSION
    INTEGER PROCEDURE FACTORIAL(N);
        VALUE N;  INTEGER N;
    BEGIN
        IF N > 1 THEN
            FACTORIAL := N*FACTORIAL(N-1);
        ELSE
            FACTORIAL = 1;
    END;
%
    STRING OUTPUT;
    INTEGER I,J;
    FOR I := 1 STEP 1 UNTIL 10 DO BEGIN
        J := FACTORIAL(I);
        OUTPUT := STR(I) & "! = " & STR(J);
        STRINGWRITE(OUTPUT);
        NEWLINE;
    END;
END.

1! = 1
2! = 2
3! = 6
4! = 24
5! = 120
6! = 720
7! = 5040

* * * * RUN TIME ERROR * * * *
* * * * ERROR NUMBER 1 * * * *

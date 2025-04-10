# TRAINING
       IDENTIFICATION DIVISION.
       PROGRAM-ID. GREATEST-OF-THREE.
       AUTHOR. CHATGPT.

       DATA DIVISION.
       WORKING-STORAGE SECTION.
       01  NUM1        PIC 9(3) VALUE ZEROS.
       01  NUM2        PIC 9(3) VALUE ZEROS.
       01  NUM3        PIC 9(3) VALUE ZEROS.
       01  GREATEST    PIC 9(3) VALUE ZEROS.

       PROCEDURE DIVISION.
       DISPLAY "Enter the first number: ".
       ACCEPT NUM1.

       DISPLAY "Enter the second number: ".
       ACCEPT NUM2.

       DISPLAY "Enter the third number: ".
       ACCEPT NUM3.
#finding largest number
       IF NUM1 > NUM2 AND NUM1 > NUM3
           MOVE NUM1 TO GREATEST
       ELSE IF NUM2 > NUM1 AND NUM2 > NUM3
           MOVE NUM2 TO GREATEST
       ELSE
           MOVE NUM3 TO GREATEST
       END-IF.

       DISPLAY "The greatest number is: " GREATEST.

       STOP RUN.

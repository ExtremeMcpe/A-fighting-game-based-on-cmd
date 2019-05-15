# A-fighting-game-based-on-cmd
paste this in your notepad and save as *.bat and run it
# code
@echo off
title [The Fighter]
color 4e
if "%1" neq "" ( goto %1)
:Menu
cls
echo                     1. Start
echo                     2. Credits
echo                     3. Exit
set /p answer=Type the number of your option and press enter : 
if %answer%==1 goto Start_verify1
if %answer%==2 goto Credits
if %answer%==3 goto Exit
:start_verify1
if exist save1.txt goto roam-1
if not exist goto start_1
if exist save2.txt goto roam-2
if not exist goto roam-1
if exist save3.txt goto roam-3
if not exist goto roam-2
if exist save4.txt goto roam-4
if not exist goto roam-3
if exist save5.txt goto roam-5
if not exist goto roam-4

:Start_1
cls
echo Oh no! You're surrounded by enemies.
echo There are five of them, and they're all armed.
echo If you fight them, you are having a high chance of winning.
set /p answer=Would you like to fight or run?
if %answer%==fight goto Fight_1
if %answer%==run goto Run_1
pause
:Run_1
cls
echo You live to fight another day.
pause
goto Start_1
:Fight_1
echo Prepare to fight.
echo The enemies suddenly rush you all at once.
set /p answer= Type 1 and press Enter to continue.
if %answer%==1 goto Fight_1_Loop
:Fight_1_Loop
set /a num=%random%
if %num% gtr 4 goto Fight_1_Loop
if %num% lss 1 goto Fight_1_Loop
if %num%==1 goto Lose_Fight_1
if %num%==2 goto Win_Fight_1
if %num%==3 goto Win_Fight_1
if %num%==4 goto Win_Fight_1
:Lose_Fight_1
cls
echo You were defeated. Play again?
pause
goto Menu
:Win_Fight_1
cls
echo You are victorious!
echo fight1 > save1.txt
goto roam-1
:roam-1
cls
echo [Roaming on the road...]
ping 127.0.0.1>nul
echo You - Hello have you seen the big gangstar building ??
ping 127.0.0.1>nul
echo Person 1 - N..[Words strucked in his troat...] No I have not saw the big gangstar building.
ping 127.0.0.1>nul
echo [You were not thinking that the person was speaking truth so you followed him]
ping 127.0.0.1>nul
echo After folowing him for a long time...
ping 127.0.0.1>nul
echo You saw the big gangstar building and got to know that the person was a member of it.
ping 127.0.0.1>nul
echo You - Hey ! wait.
ping 127.0.0.1>nul
echo [he stops]
ping 127.0.0.1>nul
echo He took his gun in his hand.
ping 127.0.0.1>nul
cls
:Start_2
cls
echo Oh no! You're surrounded by an enemy
echo  and he is armed.
echo If you fight him, you are having a high chance of winning.
set /p answer=Would you like to fight or run?
if %answer%==fight goto Fight_2
if %answer%==run goto Run_2
:Fight_2
echo Prepare to fight.
echo The enemy suddenly rush you at once.
set /p answer= Type 1 and press Enter to continue.
if %answer%==1 goto Fight_2_Loop
:Run_2
cls
echo You live to fight another day.
pause
goto Start_2

:Fight_2_Loop
set /a num=%random%
if %num% gtr 4 goto Fight_2_Loop
if %num% lss 1 goto Fight_2_Loop
if %num%==1 goto Lose_Fight_2
if %num%==2 goto Win_Fight_2
if %num%==3 goto Win_Fight_2
if %num%==4 goto Win_Fight_2
:Lose_Fight_2
cls
echo You were defeated. Play again?
pause
goto Menu
:Win_Fight_2
cls
echo You are victorious!
echo fight2 > save2.txt
del save1.txt
ping 127.0.0.1>nul
goto roam-2
:roam-2
echo [You Started climbing up stairs...]
ping 127.0.0.1>nul
:Start_3
cls
echo Oh no! You're surrounded by enemies
echo  and they all are armed.
echo If you fight them, you are having a high chance of winning.
set /p answer=Would you like to fight or run?
if %answer%==fight goto Fight_3
if %answer%==run goto Run_3
:Fight_3
echo Prepare to fight.
echo The enemy suddenly rush you at once.
set /p answer= Type 1 and press Enter to continue.
if %answer%==1 goto Fight_3_Loop
:Run_3
cls
echo You live to fight another day.
pause
goto Start_3

:Fight_3_Loop
set /a num=%random%
if %num% gtr 4 goto Fight_3_Loop
if %num% lss 1 goto Fight_3_Loop
if %num%==1 goto Lose_Fight_3
if %num%==2 goto Win_Fight_3
if %num%==3 goto Win_Fight_3
if %num%==4 goto Win_Fight_3
:Lose_Fight_3
cls
echo You were defeated. Play again?
pause
goto Menu
:Win_Fight_3
cls
echo You are victorious!
echo fight3 > save3.txt
del save2.txt
ping 127.0.0.1>nul
goto roam-3
:roam-3
cls
echo [you get to boss....]
ping 127.0.0.1>nul
echo boss - what you want?
ping 127.0.0.1>nul
echo you - My brother.
ping 127.0.0.1>nul
echo boss - who brother ?
ping 127.0.0.1>nul
echo you - Samarth Sinha
ping 127.0.0.1>nul
echo boss - Oh ! you are big brother of him ! 
ping 127.0.0.1>nul
echo boss -  to take him first fight me.
ping 127.0.0.1>nul
cls
:Start_4
cls
echo Oh no! You're surrounded by Boss
echo  and he is all armed.
echo If you fight him, you are having a high chance of winning.
set /p answer=Would you like to fight or run?
if %answer%==fight goto Fight_4
if %answer%==run goto Run_4
:Fight_4
echo Prepare to fight.
echo The boss suddenly rush you at once.
set /p answer= Type 1 and press Enter to continue.
if %answer%==1 goto Fight_4_Loop
:Run_4
cls
echo You live to fight another day.
pause
goto Start_4

:Fight_4_Loop
set /a num=%random%
if %num% gtr 4 goto Fight_4_Loop
if %num% lss 1 goto Fight_4_Loop
if %num%==1 goto Lose_Fight_4
if %num%==2 goto Win_Fight_4
if %num%==3 goto Win_Fight_4
if %num%==4 goto Win_Fight_4
:Lose_Fight_4
cls
echo You were defeated. Play again?
pause
goto Menu
:Win_Fight_4
cls
echo You are victorious!
echo fight4 > save4.txt
del save3.txt
ping 127.0.0.1>nul
goto roam-4
:roam-4
cls
echo [But, When you see the room, You see that your brother is not there.]
echo [You asked the boss]
echo You - now where is my brother !
ping 127.0.0.1>nul
echo boss - [Smiles] We have send your brother in our second base.
echo         Do you want to know where it is ?
ping 127.0.0.1>nul
echo You - Yes.
ping 127.0.0.1>nul
echo Boss - India
ping 127.0.0.1>nul
echo You - Where in India ?
ping 127.0.0.1>nul
echo boss - Uttar Pradesh
ping 127.0.0.1>nul
echo You - [Angrily] Can't you tell me clearly where !?
ping 127.0.0.1>nul
echo boss - Ok ! Ok ! in Varanasi.
ping 127.0.0.1>nul
echo You - Thats enough for me.
ping 127.0.0.1>nul
echo [You Quickly head to India as fast as you can]
ping 127.0.0.1>nul
echo [While you were heading to India...]
ping 127.0.0.1>nul
echo [You saw some people trying to kill you]
ping 127.0.0.1>nul
:Start_5
cls
echo Oh no! You're surrounded by enemies
echo  and they all are armed.
echo If you fight them, you are having a high chance of winning.
set /p answer=Would you like to fight or run?
if %answer%==fight goto Fight_5
if %answer%==run goto Run_5
:Fight_5
echo Prepare to fight.
echo The enemies suddenly rush you at once.
set /p answer= Type 1 and press Enter to continue.
if %answer%==1 goto Fight_5_Loop
:Run_5
cls
echo You live to fight another day.
pause
goto Start_5

:Fight_5_Loop
set /a num=%random%
if %num% gtr 4 goto Fight_5_Loop
if %num% lss 1 goto Fight_5_Loop
if %num%==1 goto Lose_Fight_5
if %num%==2 goto Win_Fight_5
if %num%==3 goto Win_Fight_5
if %num%==4 goto Win_Fight_5
:Lose_Fight_5
cls
echo You were defeated. Play again?
pause
goto Menu
:Win_Fight_5
cls
echo You are victorious!
echo fight5 > save5.txt
del save4.txt
ping 127.0.0.1>nul
goto roam-5
:roam-5
echo [You safely reached Varanasi, India]
ping 127.0.0.1>nul
echo [You headed to their second base]
ping 127.0.0.1>nul
echo [There you found many enemies]
:Start_6
cls
echo Oh no! You're surrounded by enemies
echo  and they all are armed.
echo If you fight them, you are having a high chance of winning.
set /p answer=Would you like to fight or run?
if %answer%==fight goto Fight_6
if %answer%==run goto Run_6
:Fight_6
echo Prepare to fight.
echo The enemies suddenly rush you at once.
set /p answer= Type 1 and press Enter to continue.
if %answer%==1 goto Fight_6_Loop
:Run_6
cls
echo You live to fight another day.
pause
goto Start_6

:Fight_6_Loop
set /a num=%random%
if %num% gtr 4 goto Fight_6_Loop
if %num% lss 1 goto Fight_6_Loop
if %num%==1 goto Lose_Fight_6
if %num%==2 goto Win_Fight_6
if %num%==3 goto Win_Fight_6
if %num%==4 goto Win_Fight_6
:Lose_Fight_6
cls
echo You were defeated. Play again?
pause
goto Menu
:Win_Fight_6
cls
echo You are victorious!
echo WIN!!! > save6.txt
del save5.txt
ping 127.0.0.1>nul
goto win
:win
cls
echo [You finally found your brother and lived happily ever again !]
goto credits
:Credits
cls
echo Credits
echo.
echo Thank you for playing [The Fighter]!
echo The game is a registered trademark of Extreme Inc.
goto Menu
:Exit
cls
echo Thanks for playing!
pause

## Lab 02

- Name:Marwa Qureshi  
- Email:qureshi.19@wright.edu

## Part 1 Answers

1. mkdir DirA
2. mkdir "Dir B"
3. It creates two directories Dir and B
4. DirA is better than Dir B because DirA is without spaces unlike Dir B.
5. mv B to DirB

## Part 2 Answers

1. First go inside DirA using the command cd DirA. Then create a file using touch test.txt
2. File contents:
```
**My name is Marwa Qureshi.
  These are the contents of a file inside the file named test.txt.
  This is in DirA..**
```

## Part 3 Answers

1. cp test.txt .hiddentext.txt
2. ls -la to list and see some details about the file

## Part 4 Answers

1. sudo adduser bob
2. /home/bob
3. yes, but through sudo command. The permission is denied with touch command
4. su bob
5. cd bob/
6. Yes because we are using bob's home directory with bob as the user. Bob is the owner therefore, he      can add files.
7. exit
8. cd

## Part 5 Answers

1. sudo addgroup crew
2. Type "sudo usermod -a -G crew bob" to add bob in the crew group.
	  Then check if bob appears in the crew group by typing "cat /etc/group".
	  Type "sudo usermod -a -G crew marwaq" to add marwaq in the crew group.
3. sudo chgrp -R crew DirA
	 This makes DirA appear in group crew
4. su bob
5. touch bob.txt
6. Yes we changed the group of DirA to crew and since bob is 
	 part of crew bob can create a file

## Part 6 Answers

1. I exit user bob and typed in the home directory the command that follows: 
	 sudo touch sudowho.txt
2. -rw-r--r-- 1 root   root
3. sudo vim sudowho.txt

## Extra Credit

1. touch mydiary.txt to create the file. Do ls -la to see the file listed with the size, dat. Change the user of the file to sally. 
2. yes, but through sudo command. The permission is denied with touch command 
3. Bob cannot go into sally's file because he is not the owner of that file, sally is. However, if Sally was to allow public access to her file then bob may be able to access it

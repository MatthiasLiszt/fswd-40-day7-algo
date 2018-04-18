#Red Ghost Algorithmn To Find Pacman

<code>
 define WayArray
 index=0

WayArray[index]="straight"
if (Pacman is reached) then goto Found
WayArray[index]="turn left"
 if (Pacman is reached) then goto Found
WayArray[index]="turn right"
 if (Pacman is reached) then goto Found

increase:
Increase WayArray By One Element and Check If Packman is reached
if(Pacman is reached) goto Found
else goto increase
 
  Found:
  print "Pacman Reached"
  End:
  END
</code>

## description

the basic idea is to start with one simple direction or motion and then 
increase the list of possible motions to find Pacman
everything possible has to be tried out  and I think it is in the order of 
3^n solutions, where the n is increasing with every added motion
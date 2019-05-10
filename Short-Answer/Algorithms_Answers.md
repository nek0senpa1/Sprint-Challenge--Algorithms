Add your answers to the Algorithms exercises here.

a) I suppose it's O(n), n is a variable, it's just going to run a specified amount of times, whatever n is

b) It's just several nested for loops, but I suppose they are still only running n number of times since it's the first in the range, which would mean several of the for's won't even run unless the n is large enough to surpass the (var) + 1's in subsequent for loops.  As for complexity... I suppose I'd go with O(n) since it's all based off the single N value

c) this is a recursive function, so bunnies is the determining factor here, if bunnies is 0 it's over, if it's one it's over in one pass.  So again I guess I'll go with O(n)

Exercise II

Alright, so we need a 'story' variable to keep track of the stories in the building.  And we'll a 'broken' boolean I suppose.  Then we'll want to go through the stories from the maximum story, working our way down to see on what story the egg doesn't crack, thus every story below the egg also would not crack.  Or we could start at the bottom story and go up until it breaks.  I guess depending on the number of stories, it would probably be faster to go from the lowest story on up, but anyway.  So something like

broken= true
story= (given value)
for i in range of highest story to lowest (or zero)
    go through (dropping) eggs at each story until it doesn't break, set broken false when it breaks
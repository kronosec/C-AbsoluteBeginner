# C-AbsoluteBeginner
C Programming Absolute Beginner's Guide, Third Edition by Greg Perry and Dean Miller

I think I'll make this a running log of lessons learned. Not a typical readme, but a decent place to store notes for now.

I've owned this book since it first came out in 2015. It may very well be that it is now available in its fourth, fifth, or even sixth edition. Hang on, I'll use the INTERNET to check. Hell yeah, still the same version. That makes it much easier to ignore the fact that in five years, I haven't made it past the second chapter. If you want to buy it, then you should. This is not an affiliate link because who cares. Just give your money to the authors. https://www.amazon.com/Programming-Absolute-Beginners-Guide-3rd/dp/0789751984.

INTRODUCTION
Super short. Literally four pages and mostly instructions on how to read a book a la Dummies style.
Ok, cool. That was easy. I'm done with the intro. Here's my review of the intro: Short. Sweet. To the point. Some reminders that I need to learn markdown so that I can really wow people with my sense of style and emphasis. A little daunting given the authors say "C can be an extremely cryptic and difficult language" but apparently you can eventually have some fun. So, the lesson I learned from this chapter is that fun is a relative term.

I'm not going to add code for the INTRO because I haven't learned any C yet. That's all I have to say about the INTRO.

CHAPTER ONE
Hard sell on C. I mean I bought the book already but sure, this is adding some motivation. Like when you buy an ice cream cone and the guy follows you out of the store and down the street going, "YOURE GONNA LOVE THAT ICE CREAM." And, in fact, I do love the ice cream. Both of those words have Cs in them and Cs get degrees (quotributed to George W. Bush). What kinds of degrees? Computer sCienCe degrees. Whoa.

Ok, materials. I need a thing called a compiler, but italicized. Hang on, I need some coffee. One thing you need to know about me is that I double fist coffee in the morning. Now, to some people, that might sound like a double entendre, but I really mean I jam both fists into a boiling pot of coffee. Really stimulates the senses, which is why I call it Five Gumming. But I digress. And I need a compiler. This book is really pushing something called Code::Blocks, but true to form, I'm going to start ignoring the advice of my teachers early on and do something else. I just downloaded Xcode because I am a MACINTOSH user (read: more tech savvy than PC users). It's almost done downloading and seems like a pretty good way to waste 8GB of space on my 12GB SSD. Still installing. Let's go back to the book. Code::Blocks is a *compiler* <-- markdown champion. Oh, wait, it's an *Integrated Development Environment* or *IDE*. I'm going to stop reading and take a wild guess that this is some kind of environment that integrates some kind of development. In a sense, it probably puts things together, or, compiles them. Great. I guess I have some sort of sick sense of tuition. 

Sweet. There are only five steps to success. Way easier than those 12 steps my family intervened me about (or zero if you know what I mean!).
1. Objective - Develop a vision board with Oprah at the center and Stanley Kubrick explaining the future on the periphery
2. Get an editor - Reach out to the good folks at Simon and Schuster. Print is dying. Throw them a bone.
3. *Compile* - Compiler I hardly know her. That joke belongs earlier in this write-up, but my brain is always playing ketchup.
4. Assume everything worked because it should on the first try or you suck
5. Profit

Error: Too many steps. Quitting.

The book would now like to brag about how efficient C is. Not just on its own, but in *relation* to other proglangs. Proglangs is an invention of KronoSec, all rites interred.

END CHAPTER ONE

REVIEW OF CHAPTER ONE - Now I know that C is confusing as hell, but better than hell, and I have an *IDE*A about how to code because of the Five Step Program. Six Stars and a Thumb.

CHAPTER TWO - The Impassable Gate
It was a cold, dark knight. We assumed he was dead. Hey does GitHub log your IP address?
Hey, this chapter is called WRITING YOUR FIRST C PROGRAM. Spoiler alert, I already did yesterday. It was as easy as copying and pasting with my eyes. This chapter also introduces something called the main() function. Last of all, I want you to know that I signed up for CS50 taught by h4Rv4r@ 2niv3r51T3. I'm a programmer now. It occurred to him as he wrote, that he was beginning far too many sentences with 'hey' and in grave danger of becoming the hilarious characature of our dearly departed Cubs announcer, Mr. Harry Caray, as portrayed by William J. Ferrell. HEY! If you were a hotdog programmed in C, would you compile yourself? Oh yeah, now I'm remembering Colin Quinn. The lovable scamp of late night. Now back to CHAPTER TWO. Actually, that's enough for one day. Bye.

CHAPTER TWO - CONTINUED
It was a day later. Sleep eluded him. He was staring at the phone when C called. Realizing now that you can't spell confusion without C. My book, |Beginner's|, shows initial C code as only requiring the main() function, but CS50 introduces the int main(void) function. After several minutes of perplexed staring, I went to StackOverflow and Carl Norum (very famous) said that main() isn't standard C and the only *real* functions, which Carl call *signatures* are int main(void) and something like int main(arcc ccc+++carccc arg). I don't know why, but I trust Carl and his 25 upvoting acolytes. Point, Harvard. If this book fails me once more, it is going into the bin.

The main() error shows in the CS50 sandbox as well. When I type:
//Prints Hello, World!
#include <stdio.h>
main()
{
    printf("Hello, World!");
}

I get yelled at. 

1 warning generated.
$ clang hello.c
hello.c:3:1: warning: type specifier missing, defaults to 'int' [-Wimplicit-int]
main()

Here's another thing. Don't be like me (at all, really) and keep calling the c file itself as if it's a compiled executable. Clanging hello.c is great. It generates the binary a.out. But remember that the binary is the thing to execute. Doing ./hello.c will result in an error like:

./hello.c: line 1: //Prints: No such file or directory
./hello.c: line 4: syntax error near unexpected token `('
./hello.c: line 4: `int main()'

Doing ./a.out will get you your Hello, World! But it will be ugly and have a $ after it until you throw in a \n before the last quotation mark.

Dot slash Dot slash Dot slash Dot slash Dot slash Dot slash Dot slash Dot slash Dot slash Dot slash Dot slash Dot slash Dot slash Dot slash Dot slash Dot slash Dot slash Dot slash Dot slash Dot slash Dot slash Dot slash Dot slash Dot slash Siri remind me to dot slash. Ok, I'll remind you to not smash...me when I hear you wrong every single time.

I'm going to move some of these more specific lessons learned into the code itself. "But that's not the purpose of comments!" a nerd cries out. Shut up, nerd. I comment what I want, where I want. Shut the hell up.

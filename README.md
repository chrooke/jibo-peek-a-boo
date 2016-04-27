#Peek-a-boo for Jibo

This is a simple peek-a-boo game suitable for young children.

Jibo introduces the game then looks away. If the kid says something, or after a random amount of time that can be configured in the skill, he'll turn back and say, "Peek-a-boo", then play an animation. Jibo will then wait for a few seconds. If the child says one of a few pre-set words, he'll announce, "I hear you!" an turn back.

If anyone says, "done", "enough, or "stop" whenever Jibo is listening, he'll finish up his animation cycle then exit the skill.

##Disclaimer
Don't let your kid drool or chew on Jibo! That can't possibly be good for anybody. Also, Jibo does move during this skill, so watch out for little fingers and such. PARENTAL SUPERVISION IS EXPECTED

While I am a parent, I have no particular child development training, and none was consulted. This skill is just for fun, and I make no claims that it will do anything to help develop your child in any meaningful way.

## Configuration

### Wait times
In the first ExecuteScript in main.bt you'll see variables for setting the minimum and maximum waiting times for when Jibo is looking away or facing you. These are in milliseconds.

### Responses
If you want to change what Jibo responds to from the child, edit rules/again.rule. Add what you want, pipe-separated, into the parentheses for the "baby=" rule.

## To Do
A little more fun with the animations, particularly the eyes.

## Known bugs
I want to trigger the "See you" sound from an animation event, but for some reason this is failing even though I've followed sample-code to a T. Maybe I'll figure this out later.

## Acknowledgments
This skill was inspired by Michael Rodriguez's "Jibo, Look Away" skill, though it uses none of his code.
This skill uses some code from the blank "Hello, world" Jibo project and some code from Jibo's sample-code.

# Version history
0.1: Initial release.
0.2: Updated for jibo-sdk 1.3.3. Slight change to timing.

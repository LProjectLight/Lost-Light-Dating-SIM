init:
    $ whirl_relationship = 0
    $ whirl_01_done = false 
    $ rung_points += 20
    $ whirl_points += 20
    $ variable -= 0
    $ variable += 0
    $ whirl_greyheart_trigger = true
    $ 12:00_2:30 = true
    $ sunny_day = true
    $ thursday = true
    $ rungs_office_unlocked = true
    $ rung_met = true
    $ whirl_met = true
    $ pause_time = true 
    $ grey_star = true
    $ whirl_idk = false
    $ whirl_guilt = false
    $ whirl_no = false
    $ whirl_cgs_1= false
   
    
label whirl_cgs_01:        
# This is Whirl's first star event, it's triggered if you gained 20 points or higher.
# Requirements:
# You must have met Rung, Rung must be at 20 points or higher, Must be on a thursday. 
# Enter Rung's office from 12:00PM to 2:30PM on a sunny day

show image whirl_se1 with fade
show bg rung_office
show rung 
show whirl

r "So, Whirl, I heard from {color=#00ff00}Ultra Magnus{/color} that you have been doing harmful things again, care to explain?"
w "None of your buisness eyebrows. I don't understand why {color=#00ff00}Magnus{/color} is such a stickler anyways. The old Mech needs to loosen up a little!"
r "Whirl, you do realize you've been doing this harmful things and you've been getting in trouble for that kind of behavior. Why do you always do bad things?"
w "Maybe because I act like this because of serious issues that I myself knows about?" 
"Whirl and Rung seemed to be talking, this was a session that you were invited by Rung to help him with Whirl's behavior. You stepped in."
r "Oh hello [player]! You must've just gotten here." 

menu: 
    "Yeah, I just gotten here.":
    jump yes
    "No, I've been here the entire time.":
    jump no
    
label yes:

r "oh that's good! Hopefully you can help me with uncovering Whirl's behavior issues, since he's talked alot about you." 

else: 
    r "Oh, that's good! You must've heard us talking, maybe you can help us try and uncover Whirl's problematic behavior. He's talked alot about you."
pass

"You nodded, you walked next to Rung and Whirl looked angry at Rung for spilling his secret." 
w "I don't want to talk with this femme in the room! I don't like her!" 
r "You did just admit you liked her." 
w "..."
hide whirl
hide rung 
"Defeated, Whirl sat back down, you decide to begin your assesment with the help of Rung."

screen input(prompt):

    window:
        has vbox

        text prompt
        input id "Welcome to your first ever Event! You must click the right things (or not) to get points!"
        
r "Alright [player] now lets start with an easy question for Whirl." 
jump choice_idk

label choice_idk:

menu:
    "Why are you ike this?":
    $ whirl_relationship -= 1 
    jump whirl_idk 
    "Do you ever feel bad for the things you do?":
    $ whirl_relationship -= 3 
    jump whirl_guilt 
    "Were you always like this?":
    $ whirl_relationship += 4
    jump whirl_no
    
 label choice_guilt: 

menu:
  "Do you ever feel bad for the things you do?":
    $ whirl_relationship -= 3 
    jump whirl_guilt 
    "Were you always like this?":
    $ whirl_relationship += 4
    jump whirl_no
    
  label choice_no:
  
 menu:
    "Were you always like this?":
    $ whirl_relationship += 4
    jump whirl_no
    
 label choice_idk_alt:
 
 menu:
      "Why are you ike this?":
    $ whirl_relationship -= 1 
    jump whirl_idk 
    "Were you always like this?":
    $ whirl_relationship += 4
    jump whirl_no
    
   label choice_guilt_alt:
   
   menu:
    "Do you ever feel bad for the things you do?":
    $ whirl_relationship -= 3 
    jump whirl_guilt 
    "Were you always like this?":
    $ whirl_relationship += 4
    jump whirl_no
    
    label choice_no_alt:
    
    menu:
    "Why are you ike this?":
    $ whirl_relationship -= 1 
    jump whirl_idk 
    "Do you ever feel bad for the things you do?":
    $ whirl_relationship -= 3 
    jump whirl_guilt  
    
 label whirl_idk:
  $ whirl_idk = true
  show whirl
 
 w "Do you want me to give you the REAL reason why I'm like this? Or do you want me to completely cry? I don't know why you're asking me these questions."
 w "What happened, happened, I even told Eyebrows over here, i don't care about my situation. I'm pretty sure he doesn't care either."
 w "But he's just caring cause he's obliged to do so."
 "Whirl narowed his one optic towards Rung."
 w "In any case, Give me the next question.
 hide whirl

 if whirl_guilt == false:
 jump choice_guilt
 if whirl_guilt true: 
 jump choice_guilt_alt
 
 if whirl_no == false: 
 jump choice_no
 if whirl_no == true: 
 jump choice_no_alt
 
label whirl_guilt: 
$ whirl_guilt = true 
show whirl
 
w "If I really felt bad I would've have repented to {color=#00ff00}Primus{/color} a long time ago. But I don't really feel bad."
w "What done was done. I have no regrets and even if I did, I couldn't change the fact I did what I did all those vorns back."
w "It's just a sad fact I have to live by. And sometimes its the things that do count that matters." 
hide whirl

if whirl_idk == false: 
jump choice_idk_alt
if whirl_idk == true:
jump whirl_idk_false

 if whirl_no == false: 
 jump choice_no
 if whirl_no == true: 
 jump choice_no_alt
 
 label whirl_no: 
 $ whirl_no = true
 show whirl
 
 "Whirl at that question looked saddened, he tried to hide it, but it was hard for you to believe his lies."
 w "I wasn't always like this [player]."
 pause
 pause 
 pause
 w "I used to have a face..."
 pause 
 pause
 pause
 w "But that was all taken away, after I REFUSED to do what they ordered."
 pause
 pause
 w "You see I was a victim of unjust torture called the empurata, it was a ritual where they took everything that you love..."
 pause
 w "And turned you into what you see now."
 w "The only reason why they did this was because I refused to protect them..."
 pause 
 pause
 pause
 w "I lost everything... I can no longer make clocks, my purpose was ruined."
 w "Although the procedure is no longer legal..." 
 pause
 pause
 pause
 pause
 w "I feel damn bad for those poor unfortnate souls." 
 
 hide whirl with fade
 hide rung_office with fade
 scene whirl_cgs_1 with fade
 
 "You pulled Whirl into a small hug."
 "He didn't want to hug you at first..."
 pause
 pause
 pause
 pause
 pause 
 "But he gradually allowed it."
 pause 
 pause
 
 mc "Whirl..."
 menu: 
 "I'm sorry...":
 jump sorry
 
 label sorry:
 "Whirl didn't say anything, he was silent." 
 "You heard what seemed to be like... Crying?"
 w "You don't have to be sorry, [player]. I put myself into this mess." 
 w "I shouldn't have to have people feel sorry for me."
 w "It isn't right." 
 pause 
 pause
 w "When you truly feel alone like i have, you depend solely on yourself." 
 w "You shun others because they were naive creatures that hasn't been through what you've been through." 
 pause
 w "You can say I was trying to protect others."
 w "...Hah... So much for being tough..." 
 "Whirl pulled away from the hug."
 
 scene rung_office with fade
 show whirl
 $ whirl_cgs_1 = true 
 
 w "Well, I shouldn't be as embarassed as I should feel... I guess I needed to feel that way. Thanks [player]..." 
 $ whirl_relationship += 10
 
 return

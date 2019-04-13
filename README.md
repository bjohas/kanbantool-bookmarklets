# kanbantool-bookmarklets

This is a bookmarklet that switches from the board (or any of the settings pages for a board) to "power ups". 

javascript: var dest = "powerups"; /* card_types, card_template, workflow, powerups, automation_rules  */ var a=document.location + " "; if ( !a.match(/kanbantool\.com\/b\/\d+/)) { alert("You have to be on a Kanbantool.org board for this to work!"); } else { a=a.replace(/(\/b\/\d+)(\/|\-| ).*$/,"$1"); document.location=a+"/"+dest; };


The string 

dest = "powerups"; 

can be any of 

card_types, card_template, workflow, powerups, automation_rules

or indeed "" to get back to the board itself (though that button is always present). The bookmarklet thus allows one to switch e.g. from the board directly to automation, rather than having to click settings first, then automation.



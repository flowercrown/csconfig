echo "====================xxxxxxxxxxx  autoexec start  xxxxxxxxxxx===================="

sensitivity "2.400000"
zoom_sensitivity_ratio_mouse "1" 

bind "/" "slot2"
bind "," "slot1"
bind "UPARROW" "slot3"
bind "h" "+left"
bind "j" "+back"
bind "k" "+right"
bind "u" "+forward"
bind "i" "+use"
bind "6" "buy flashbang; slot7;"
bind "9" "buy hegrenade; slot6;"
bind "7" "buy incgrenade; buy molotov; slot10;"
bind "8" "buy smokegrenade; slot8;"
bind "MWHEELUP" "slot3"
bind "d" "use weapon_Taser"
bind "p" "buymenu"
bind "o" "+reload"
bind "MWHEELDOWN" "+jump"
bind "c" "+duck"
bind "v" "+sprint"
bind "MOUSE1" "+attack;r_cleardecals"
bind "MOUSE2" "+attack2"
bind "MOUSE3" "slot5"
bind "MOUSE4" "+voicerecord"
bind "MOUSE5" "drop"


cl_crosshairalpha "255"
cl_crosshaircolor "5"
cl_crosshaircolor_b "90"
cl_crosshaircolor_r "90"
cl_crosshaircolor_g "250"
cl_crosshairdot "0"
//cl_crosshairgap "-14"
cl_crosshairgap "-0.2"
//cl_crosshairsize "2"
cl_crosshairstyle "4"
cl_crosshairusealpha "1"
//cl_crosshairthickness "1.5"
cl_fixedcrosshairgap "-14"
cl_crosshair_outlinethickness "1"
cl_crosshair_drawoutline "1"
cl_crosshairsize "1.117293"
cl_crosshairthickness "1.1"

bind space "exec jumpthrow"

//tap jumpthrow
alias +fjt "+forward; +jump;"
alias -fjt "-jump; -forward;"
alias +fjtRelAttack "-attack;-attack2;"
bind "f" "+fjt; +fjtRelAttack"

//crouchjump bind
//alias "+hjump" "+jump; +duck"; alias "-hjump" "-jump; -duck"; bind rshift "+hjump"

//radar
cl_radar_square_with_scoreboard false
cl_radar_scale 0.4
cl_radar_icon_scale_min 0.2

snd_remove_soundevent Flashbang.Ring.Short; 
snd_remove_soundevent Flashbang.Ring.Long; 
snd_remove_soundevent Flashbang.Ring.Medium;

host_writeconfig

echo "====================!!!!!!!!!!!!!autoexec executed!!!!!!!!!!!!!===================="

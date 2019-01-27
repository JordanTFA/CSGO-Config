# CSGO-Config
My autoexec configuration for CounterStrike: Global Offensive

// =====================
// = PEW PEW BANG BANG =
// =====================

bind kp_uparrow "say pew pew bang bang"

// =====================
// ==== SHOW STATS =====
// =====================

con_filter_text damage
con_filter_text_out Player:
con_filter_enable 2
developer 1

// =====================
// ==== JUMP THROW =====
// =====================

alias "+jumpthrow" "+jump;-attack"
alias "-jumpthrow" "-jump"
bind "h" "+jumpthrow"

alias "+runthrow" "+forward;+jump;-attack" 
alias "-runthrow" "-jump;-forward" 
bind "j" "+runthrow"


// ======================
// ==== SHIFT VOLUME ====
// ======================

alias +walkvol "+speed; volume .3; voice_scale 0.3"
alias -walkvol "-speed; volume .1; voice_scale 1"
bind shift +walkvol

// ======================
// == EVERYTHING BIND ===
// ======================

bind "p" "bot_kick;sv_cheats 1;sv_infinite_ammo 1;sv_grenade_trajectory 1;sv_showimpacts 1;mp_roundtime_defuse 60;mp_afterroundmoney 16000; mp_buy_anywhere 1;mp_buytime 9999;give weapon_ak47;give weapon_smokegrenade;give weapon_flashbang;give weapon_molotov"


// ======================
// ===== FIND BOMB ======
// ======================

alias "+findbomb" "+use; gameinstructor_enable 1" alias "-findbomb" "-use; gameinstructor_enable 0" bind "E" "+findbomb"
bindtoggle x gameinstructor_enable

// ======================
// ======= SOUND ========
// ======================

snd_mixahead "0.05"
snd_headphone_pan_exponent "2"
snd_musicvolume "0"

// ======================
// ====== GRENADES ======
// ======================

bind 4 "use weapon_hegrenade"
bind "mouse3" "use weapon_flashbang"
bind "mwheelup" "use weapon_smokegrenade"
bind "mouse4" "use weapon_molotov"

// ======================
// ===== CROSSHAIR ======
// ======================

cl_crosshairalpha "255"
cl_crosshaircolor "4"
cl_crosshaircolor_b "0"
cl_crosshaircolor_r "255"
cl_crosshaircolor_g "0"
cl_crosshairdot "0"
cl_crosshairgap "0"
cl_crosshairsize "3"
cl_crosshairstyle "5"
cl_crosshairusealpha "1"
cl_crosshairthickness "0.5"
cl_fixedcrosshairgap "0"
cl_crosshair_outlinethickness "1"
cl_crosshair_drawoutline "1"

// ======================
// ======= STUFF ========
// ======================

bind c "use weapon_c4; drop"
bind "t" noclip
bind "f" +lookatweapon; r_cleardecals;
cl_disablehtmlmotd 1
voice_enable 1
net_graphproportionalfont 0
cl_autowepswitch "0"
cl_showloadout 0
+cl_show_team_equipment 1

alias +shownet "+showscores; net_graphheight 64"
alias -shownet "-showscores; net_graphheight 9999"
net_graph 1
bind TAB +shownet

// ======================
// ===== JORDAN LAND ====
// ======================

sensitivity 2

bind "mouse5" +voicerecord
bind "mwheeldown" +jump
bind "ctrl" +duck

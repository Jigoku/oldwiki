These are the variable changes from version 1.3.1 to 1.4, deletions are marked in red with a strike-over, additions are marked in green with underline, unchanged context are plain black.

This page was created by

-   Executing the writevars command in the two Red Eclipse versions being compared

`./redeclipse.sh -hhome1 -x'writevars "vars.txt" 1; quit'`
`./redeclipse.sh -hhome2 -x'writevars "vars.txt" 1; quit'`

-   Adding the first version to a git staging area and then overwriting with the second version (git has the most useful word-diff it seems)

`cd home1`
`git init`
`git add vars.txt`
`cp ../home2/vars.txt .`

-   Executing this command to compare and format the output

<!-- -->

    <nowiki>git diff --word-diff=plain \
    | sed -n 's%\([[{+-]*\)// % \1%gp' \
    | sed 's%\[-%<span style="color:red; text-decoration:line-through">%g' \
    | sed 's%-\]%</span>%g' \
    | sed 's%{+%<span style="color:green; text-decoration:underline">%g' \
    | sed 's%+}%</span>%g' \
     >wikipage.txt</nowiki>

`actorscale 1.0`
<span style="color:red; text-decoration:line-through">`aircoastforce -1.0`</span><span style="color:green; text-decoration:underline">`aiinitdelay 5000`</span>
<span style="color:green; text-decoration:underline">`ailongdelay 10000`</span>
<span style="color:green; text-decoration:underline">`aircoast 25.0`</span>
`aircoastscale 1.0`
<span style="color:green; text-decoration:underline">`airefreshdelay 1000`</span>
<span style="color:green; text-decoration:underline">`allowlock 4`</span>
<span style="color:green; text-decoration:underline">`allowmaps "ares bath battlefield biolytic bloodlust canals cargo center colony conflict cutec cyanide darkness deadsimple deathtrap deli depot dropzone dutility echo erosion error forge foundation fourplex futuresport ghost hawk hinder institute keystone2k linear livefire longestyard mist neodrive nova oneiroi panic processing pumpstation purge spacetech starlibido stone suspended testchamber tower tranquility tribal ubik vault venus warp wet"`</span>
`assistkilldelay 5000`
<span style="color:green; text-decoration:underline">`autoadmin 0`</span>
<span style="color:green; text-decoration:underline">`autospecdelay 60000`</span>
<span style="color:green; text-decoration:underline">`autospectate 1`</span>
<span style="color:green; text-decoration:underline">`balancedelay 10000`</span>
<span style="color:green; text-decoration:underline">`balancemaps -1`</span>
<span style="color:green; text-decoration:underline">`balancenospawn 1`</span>
<span style="color:green; text-decoration:underline">`banlock 4`</span>
`bleeddamage 3`
`bleeddelay 1000`
`bleedtime 5500`
`bomberbuffdamage 1.5`
`bomberbuffdelay 1000`
`bomberbuffing 1`
`bomberbuffshield 1.5`
`bombercarryspeed `<span style="color:red; text-decoration:line-through">`0.75`</span><span style="color:green; text-decoration:underline">`0.9`</span>
`bombercarrytime 15000`
`bombercollide `<span style="color:red; text-decoration:line-through">`2`</span><span style="color:green; text-decoration:underline">`64`</span>
`bomberdelay 3000`
`bomberdelta 1000.0`
`bomberelasticity `<span style="color:red; text-decoration:line-through">`0.65`</span><span style="color:green; text-decoration:underline">`0.7`</span>
`bomberextinguish 6`
`bomberholdinterval 1000`
`bomberholdlimit 0`
`bomberholdpenalty 10`
`bomberholdpoints 1`
<span style="color:green; text-decoration:underline">`bomberholdtime 15000`</span>
<span style="color:green; text-decoration:underline">`bomberinteracts 3`</span>
`bomberlimit 0`
`bomberlockondelay 250`
<span style="color:green; text-decoration:underline">`bombermaps "ares battlefield biolytic canals cargo center colony conflict cutec darkness deadsimple deli depot dropzone dutility echo erosion foundation fourplex futuresport ghost linear mist nova pumpstation stone suspended tower tribal vault venus warp wet"`</span>
`bomberminspeed 50.0`
`bomberpenalty 5`
`bomberpickupdelay 5000`
`bomberregendelay 1000`
`bomberregenextra 2`
`bomberrelativity 0.25`
<span style="color:red; text-decoration:line-through">`bomberreset 0`</span>
`bomberresetdelay 15000`
`bomberspeed `<span style="color:red; text-decoration:line-through">`250.0`</span><span style="color:green; text-decoration:underline">`200.0`</span>
`bomberthreshold 0.0`
`bomberwaterfric 1.75`
`bomberweight `<span style="color:red; text-decoration:line-through">`150.0`</span><span style="color:green; text-decoration:underline">`200.0`</span>
`botbalance -1`
<span style="color:green; text-decoration:underline">`botfemalenames "sue debbie luanne brandy angel kitty jane ava brianna chloe destiny emma faith grace hannah julia kaylee lily madison natalie olivia peyton riley sophia taylor unique victoria ximena yaretzi zoe avdotya aurora agatha agafya agnes ada adelaide adeline adele adriana aksinya alevtina alain alina alice aliyah alla alsou alba albina alfia alya amalia amin amir anahit anastasia angelina angela angelica anisa anna antonina anfisa arina bela bertha valentine valeria varvara vasilisa veronica victoria vilena violet vita vitalina galina ghalia greta gulmira dana daniela dara darina daria jamila diana dilara dinara eve eugene evdokia catherine helena elizabeth yesenia jeanne jasmine josephine zaire zamira zara sarin zemfira zinaida zoe zulfiya zukhra ilona inga inessa inna john ira iraida irene irma kamila camilla karina caroline kira claudia clara bark cornelia christina xenia lada lana larissa laura leila lera lesya liana lika lillian lily lina linda liora lyra laura ludmila magdalena mara margaret marianne marika maria martha mika milena milica monica naila naima naomi natalia nelly nick nicole nina ninel nora nuria oksana olesya olga peacock paula pelagia platonida pauline praskovya rada razin raisa regina mignonette rena renata rihanna rina rita rogneda rose rusalina sabrina sandra sarah sati safura svetlana seraphim sylvia snezana sophia stella stephanie susanna taisa tamara tara teresa tina ulyana ursula feruza firouz flora florentina florian shakira sheila shelley evelina evita eleanor eliana eliza elina ella elvina elmira elnara emma ermina ethel eter julia jadwiga jana yanina yasmin yaroslav jasmina"`</span>
<span style="color:green; text-decoration:underline">`botfemalevanities "badge"`</span>
<span style="color:green; text-decoration:underline">`botmalenames "moe larry curly jerry ted phil bob billy joe john james gunner dante dick lorenzo chuck zeus alexander benjamin daniel ethan fernando gabriel hunter isaac jacob kevin logan michael noah owen parker ryan samuel tyler uriel victor william xavier yahir zachary abram avaz abraham agap agapit agathon adam adrian azamat azat aidar airat akim alan alexander alex ali alikhan diamond albert anatoly angel andrew anton anfim aram arkady arman armen arseniy arslan artem artemia arthur askhana ahmet ashot bahram bogdan boris borislav bronislaw damask vadim valentine valery waldemar vardan vasily victor william wit vitali vladimir vladislav vladlen vsevolod vyacheslav hamlet harry gennady henry henry george gerasim herman hermann gleb gordi gregory gustav david dawlat damir dana daniel danislav denis jamal james jeremy jeremiah joseph dick dinar dino dmitry dobrynya eugene evdokim eustace yegor elisha emelyan jeremiah yefim ephraim zhdan zakir zachar zinovy ibrahim ivan ignat ignatius igor jerome ilshat ilya innocent isaac isaac isidore iskander ismail kazbek camille karen karim charles kim cyril klaus klim conrad constantine cornelius kuzma leo leon leonard leonid leopold luke lukillian lukjan lubomir ludwig louis lucius michael makar macarius maxim maximilian maqsood mansour march marat mark marseilles martin matthew mahmoud mika mikula miron miroslav michael mstislav murat mohammed nazar nikita nicodemus nicola nicholas nils oleg orlando oscar ostap paul pedro peter plato prokhor ravil radium radik radomir radoslav razil raymond ramiz ramil ramon ranelagh ratmir raphael richard robert rodion roland rostislav rudolph ruslan rustam ray sawa savely samuel svyatoslav sebastian sergei stepan tamerlan taras fedor felix philip fred frederick shamil charles edgar edward eldar julian julius yuri jacob yaroslav"`</span>
<span style="color:green; text-decoration:underline">`botmalevanities "badge"`</span>
`botoffset 0`
`botscale 1.0`
`botskillmax 75`
`botskillmin `<span style="color:red; text-decoration:line-through">`50`</span><span style="color:green; text-decoration:underline">`60`</span>
`botspeed 1.0`
`burndamage 3`
`burndelay 1000`
`burntime 5500`
`capturebuffarea `<span style="color:red; text-decoration:line-through">`3.0`</span><span style="color:green; text-decoration:underline">`96.0`</span>
`capturebuffdamage 1.5`
`capturebuffdelay 1000`
`capturebuffing 5`
`capturebuffshield 1.5`
`capturecarryspeed 0.9`
`capturecollide `<span style="color:red; text-decoration:line-through">`2`</span><span style="color:green; text-decoration:underline">`64`</span>
`capturedefenddelay 15000`
`captureelasticity `<span style="color:red; text-decoration:line-through">`0.35`</span><span style="color:green; text-decoration:underline">`0.5`</span>
`captureextinguish 6`
<span style="color:green; text-decoration:underline">`captureinteracts 3`</span>
`capturelimit 0`
<span style="color:green; text-decoration:underline">`capturemaps "ares bath battlefield biolytic canals cargo center colony conflict cutec darkness deadsimple deli depot dropzone dutility echo erosion foundation fourplex futuresport ghost institute keystone2k linear mist nova panic pumpstation stone suspended tribal vault venus warp wet"`</span>
`captureminspeed 0.0`
`capturepickupdelay 5000`
`capturepickuppoints 3`
`captureresetdelay 30000`
`capturethreshold 0.0`
`capturewaterfric 1.75`
`captureweight `<span style="color:red; text-decoration:line-through">`100.0`</span><span style="color:green; text-decoration:underline">`200.0`</span>
<span style="color:green; text-decoration:underline">`connectlock 0`</span>
`coopbalance `<span style="color:red; text-decoration:line-through">`2`</span><span style="color:green; text-decoration:underline">`1.5`</span>
<span style="color:green; text-decoration:underline">`coopmultibalance 2.0`</span>
`coopskillmax `<span style="color:red; text-decoration:line-through">`95`</span><span style="color:green; text-decoration:underline">`85`</span>
`coopskillmin 75`
<span style="color:red; text-decoration:line-through">`criticalchance 100`</span>
`damagescale 1.0`
`deadpushscale 2.0`
<span style="color:green; text-decoration:underline">`deadstunscale 2.0`</span>
<span style="color:green; text-decoration:underline">`defaultmap ""`</span>
<span style="color:green; text-decoration:underline">`defaultmode 2`</span>
<span style="color:green; text-decoration:underline">`defaultmuts 0`</span>
`defendbuffdamage 1.5`
`defendbuffdelay 1000`
`defendbuffing 1`
`defendinterval 50`
`defendking 25`
`defendlimit 0`
<span style="color:green; text-decoration:underline">`defendmaps "ares bath battlefield biolytic canals cargo center colony conflict cutec darkness deadsimple deli depot dropzone dutility echo erosion foundation fourplex futuresport ghost institute keystone2k linear livefire mist nova panic processing pumpstation stone suspended tower tribal ubik vault venus warp wet"`</span>
`defendoccupy 100`
`defendpoints 1`
`defendregenbuff 1`
`defendregendelay 1000`
`defendregenextra 2`
<span style="color:green; text-decoration:underline">`demoautorec 1`</span>
<span style="color:green; text-decoration:underline">`democount 5`</span>
<span style="color:green; text-decoration:underline">`demokeep 0`</span>
<span style="color:green; text-decoration:underline">`demolock 4`</span>
<span style="color:green; text-decoration:underline">`demomaxsize 16`</span>
`dominatecount 5`
`dominatepoints 1`
`duelclear 1`
`duelcycle 2`
`duelcycles `<span style="color:red; text-decoration:line-through">`3`</span><span style="color:green; text-decoration:underline">`2`</span>
`duellimit 5000`
<span style="color:green; text-decoration:underline">`duelmaps "bath bloodlust darkness deadsimple dutility echo fourplex ghost longestyard livefire stone panic vault wet"`</span>
`duelprotect 5000`
`duelreset 1`
<span style="color:green; text-decoration:underline">`duelwarmup 15000`</span>
<span style="color:green; text-decoration:underline">`editlock 4`</span>
`enemybalance 1`
`enemybonus 1`
<span style="color:green; text-decoration:underline">`enemylimit 32`</span>
`enemyscale 1.0`
`enemyskillmax `<span style="color:red; text-decoration:line-through">`85`</span><span style="color:green; text-decoration:underline">`80`</span>
`enemyskillmin 65`
`enemyspawndelay 1000`
<span style="color:green; text-decoration:underline">`enemyspawndistmax 512.0`</span>
<span style="color:green; text-decoration:underline">`enemyspawndistmin 32.0`</span>
`enemyspawnstyle 1`
`enemyspawntime 30000`
`enemyspeed 1.0`
`enemystrength 1.0`
<span style="color:red; text-decoration:line-through">`explodelimited 0.5`</span>
<span style="color:red; text-decoration:line-through">`explodescale 1.0`</span>
`firstbloodpoints 1`
`flameradd `<span style="color:red; text-decoration:line-through">`25`</span>
<span style="color:red; text-decoration:line-through">`flameradelay1 100`</span>
<span style="color:red; text-decoration:line-through">`flameradelay2 500`</span><span style="color:green; text-decoration:underline">`30`</span>
`flameraidist1 64.0`
`flameraidist2 128.0`
`flameraiskew1 10`
`flameraiskew2 10`
<span style="color:red; text-decoration:line-through">`flamerallowed 2`</span><span style="color:green; text-decoration:underline">`flamerattackdelay1 125`</span>
<span style="color:green; text-decoration:underline">`flamerattackdelay2 1000`</span>
`flamercarried 1`
`flamercollide1 `<span style="color:red; text-decoration:line-through">`70`</span><span style="color:green; text-decoration:underline">`84`</span>
`flamercollide2 `<span style="color:red; text-decoration:line-through">`74`</span><span style="color:green; text-decoration:underline">`12316`</span>
`flamercolour `<span style="color:red; text-decoration:line-through">`0xFF2222`</span><span style="color:green; text-decoration:underline">`0xF02020`</span>
`flamercooked1 0`
`flamercooked2 1`
<span style="color:red; text-decoration:line-through">`flamercritdash1 0`</span>
<span style="color:red; text-decoration:line-through">`flamercritdash2 0`</span>
<span style="color:red; text-decoration:line-through">`flamercritdist 64.0`</span>
<span style="color:red; text-decoration:line-through">`flamercritmult 4.0`</span>
`flamerdamage2 `<span style="color:red; text-decoration:line-through">`5`</span><span style="color:green; text-decoration:underline">`4`</span>
`flamerdelta1 10.0`
`flamerdelta2 10.0`
<span style="color:red; text-decoration:line-through">`flameredelay1 200`</span><span style="color:green; text-decoration:underline">`flamerdrill1 0`</span>
<span style="color:red; text-decoration:line-through">`flameredelay2 200`</span><span style="color:green; text-decoration:underline">`flamerdrill2 0`</span>
`flamerelasticity1 0.5`
`flamerelasticity2 0.35`
<span style="color:green; text-decoration:underline">`flamerescapedelay1 200`</span>
<span style="color:green; text-decoration:underline">`flamerescapedelay2 200`</span>
`flamerexplcol1 -1`
`flamerexplcol2 -1`
`flamerexplode1 `<span style="color:red; text-decoration:line-through">`10`</span><span style="color:green; text-decoration:underline">`8.0`</span>
`flamerexplode2 `<span style="color:red; text-decoration:line-through">`10`</span><span style="color:green; text-decoration:underline">`12.0`</span>
`flamerextinguish1 3`
`flamerextinguish2 3`
`flamerflakcollide1 `<span style="color:red; text-decoration:line-through">`70`</span><span style="color:green; text-decoration:underline">`84`</span>
`flamerflakcollide2 `<span style="color:red; text-decoration:line-through">`74`</span><span style="color:green; text-decoration:underline">`12316`</span>
<span style="color:red; text-decoration:line-through">`flamerflakdmg1 12`</span><span style="color:green; text-decoration:underline">`flamerflakdamage1 4`</span>
<span style="color:red; text-decoration:line-through">`flamerflakdmg2`</span><span style="color:green; text-decoration:underline">`flamerflakdamage2`</span>` 4`
<span style="color:red; text-decoration:line-through">`flamerflakffwd1 0.5`</span><span style="color:green; text-decoration:underline">`flamerflakdelta1 10.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakdelta2 10.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakdrill1 0`</span>
<span style="color:red; text-decoration:line-through">`flamerflakffwd2`</span><span style="color:green; text-decoration:underline">`flamerflakdrill2 0`</span>
<span style="color:green; text-decoration:underline">`flamerflakelasticity1`</span>` 0.5`
<span style="color:green; text-decoration:underline">`flamerflakelasticity2 0.35`</span>
<span style="color:green; text-decoration:underline">`flamerflakexplcol1 -1`</span>
<span style="color:green; text-decoration:underline">`flamerflakexplcol2 -1`</span>
<span style="color:green; text-decoration:underline">`flamerflakexplode1 8.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakexplode2 12.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakextinguish1 3`</span>
<span style="color:green; text-decoration:underline">`flamerflakextinguish2 3`</span>
<span style="color:green; text-decoration:underline">`flamerflakguided1 0`</span>
<span style="color:green; text-decoration:underline">`flamerflakguided2 0`</span>
<span style="color:green; text-decoration:underline">`flamerflakguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`flamerflakguideddelay2 0`</span>
<span style="color:green; text-decoration:underline">`flamerflakheadmin1 4.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakheadmin2 4.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakhitpush1 5.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakhitpush2 10.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakinteracts1 1`</span>
<span style="color:green; text-decoration:underline">`flamerflakinteracts2 1`</span>
<span style="color:green; text-decoration:underline">`flamerflaklegdamage1 0.25`</span>
<span style="color:green; text-decoration:underline">`flamerflaklegdamage2 0.25`</span>
`flamerflakminspeed2 `<span style="color:red; text-decoration:line-through">`25.0`</span><span style="color:green; text-decoration:underline">`50.0`</span>
<span style="color:red; text-decoration:line-through">`flamerflakoffset1 8.0`</span><span style="color:green; text-decoration:underline">`flamerflakpartcol1 -1`</span>
<span style="color:red; text-decoration:line-through">`flamerflakoffset2 8.0`</span><span style="color:green; text-decoration:underline">`flamerflakpartcol2 -1`</span>
<span style="color:green; text-decoration:underline">`flamerflakpartlen1 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakpartlen2 5.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakpartsize1 10.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakpartsize2 10.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakparttype1 5`</span>
<span style="color:green; text-decoration:underline">`flamerflakparttype2 5`</span>
<span style="color:green; text-decoration:underline">`flamerflakproxdelay1 0`</span>
<span style="color:green; text-decoration:underline">`flamerflakproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`flamerflakproxdist1 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakproxdist2 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`flamerflakproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`flamerflakproxtype1 0`</span>
<span style="color:green; text-decoration:underline">`flamerflakproxtype2 0`</span>
<span style="color:green; text-decoration:underline">`flamerflakradial1 20`</span>
<span style="color:green; text-decoration:underline">`flamerflakradial2 20`</span>
<span style="color:green; text-decoration:underline">`flamerflakradius1 1.5`</span>
<span style="color:green; text-decoration:underline">`flamerflakradius2 1.5`</span>
<span style="color:green; text-decoration:underline">`flamerflakreflectivity1 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakreflectivity2 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakresidual1 1`</span>
<span style="color:green; text-decoration:underline">`flamerflakresidual2 1`</span>
<span style="color:green; text-decoration:underline">`flamerflakselfdamage1 0.3`</span>
<span style="color:green; text-decoration:underline">`flamerflakselfdamage2 0.3`</span>
<span style="color:green; text-decoration:underline">`flamerflakstunfall1 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakstunfall2 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakstunscale1 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakstunscale2 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakstuntime1 0`</span>
<span style="color:green; text-decoration:underline">`flamerflakstuntime2 0`</span>
<span style="color:green; text-decoration:underline">`flamerflaktaper1 1`</span>
<span style="color:green; text-decoration:underline">`flamerflaktaper2 1`</span>
<span style="color:green; text-decoration:underline">`flamerflaktaperin1 0.5`</span>
<span style="color:green; text-decoration:underline">`flamerflaktaperin2 0.5`</span>
<span style="color:green; text-decoration:underline">`flamerflaktaperout1 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerflaktaperout2 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakteampenalty1 1.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakteampenalty2 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerflaktorsodamage1 0.45`</span>
<span style="color:green; text-decoration:underline">`flamerflaktorsodamage2 0.45`</span>
<span style="color:green; text-decoration:underline">`flamerflakvisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakvisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakvistime1 0`</span>
<span style="color:green; text-decoration:underline">`flamerflakvistime2 0`</span>
<span style="color:green; text-decoration:underline">`flamerflakwaterfric1 1.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakwaterfric2 1.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakwavepush1 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakwavepush2 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakweight1 200.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakweight2 100.0`</span>
<span style="color:green; text-decoration:underline">`flamerflakwhipdamage1 0.65`</span>
<span style="color:green; text-decoration:underline">`flamerflakwhipdamage2 0.65`</span>
<span style="color:green; text-decoration:underline">`flamerfragdelay1 0`</span>
<span style="color:green; text-decoration:underline">`flamerfragdelay2 0`</span>
<span style="color:green; text-decoration:underline">`flamerfragjump1 0.5`</span>
<span style="color:green; text-decoration:underline">`flamerfragjump2 0.5`</span>
<span style="color:green; text-decoration:underline">`flamerfragoffset1 4.0`</span>
<span style="color:green; text-decoration:underline">`flamerfragoffset2 4.0`</span>
<span style="color:red; text-decoration:line-through">`flamerflakrays1`</span><span style="color:green; text-decoration:underline">`flamerfragrays1`</span>` 5`
<span style="color:red; text-decoration:line-through">`flamerflakrays2`</span><span style="color:green; text-decoration:underline">`flamerfragrays2`</span>` 5`
<span style="color:red; text-decoration:line-through">`flamerflakrel1`</span><span style="color:green; text-decoration:underline">`flamerfragrel1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`flamerflakrel2`</span><span style="color:green; text-decoration:underline">`flamerfragrel2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`flamerflakscale1`</span><span style="color:green; text-decoration:underline">`flamerfragscale1`</span>` 0.5`
<span style="color:red; text-decoration:line-through">`flamerflakscale2`</span><span style="color:green; text-decoration:underline">`flamerfragscale2`</span>` 0.5`
<span style="color:red; text-decoration:line-through">`flamerflakskew1`</span><span style="color:green; text-decoration:underline">`flamerfragskew1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`flamerflakskew2`</span><span style="color:green; text-decoration:underline">`flamerfragskew2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`flamerflakspeed1`</span><span style="color:green; text-decoration:underline">`flamerfragspeed1`</span>` 200`
<span style="color:red; text-decoration:line-through">`flamerflakspeed2`</span><span style="color:green; text-decoration:underline">`flamerfragspeed2`</span>` 250`
<span style="color:red; text-decoration:line-through">`flamerflakspread1`</span><span style="color:green; text-decoration:underline">`flamerfragspread1`</span>` 0.1`
<span style="color:red; text-decoration:line-through">`flamerflakspread2`</span><span style="color:green; text-decoration:underline">`flamerfragspread2`</span>` 0.1`
<span style="color:red; text-decoration:line-through">`flamerflaktime1`</span><span style="color:green; text-decoration:underline">`flamerfragtime1`</span>` 1000`
<span style="color:red; text-decoration:line-through">`flamerflaktime2`</span><span style="color:green; text-decoration:underline">`flamerfragtime2`</span>` 3000`
<span style="color:red; text-decoration:line-through">`flamerflakweap1`</span><span style="color:green; text-decoration:underline">`flamerfragweap1`</span>` -1`
<span style="color:red; text-decoration:line-through">`flamerflakweap2`</span><span style="color:green; text-decoration:underline">`flamerfragweap2`</span>` -1`
`flamerfrequency 1.0`
`flamerfullauto1 1`
`flamerfullauto2 0`
<span style="color:red; text-decoration:line-through">`flamergdelay1 0`</span>
<span style="color:red; text-decoration:line-through">`flamergdelay2 0`</span>
`flamerguided1 0`
`flamerguided2 0`
<span style="color:green; text-decoration:underline">`flamerguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`flamerguideddelay2 0`</span>
`flamerheadmin1 4.0`
`flamerheadmin2 4.0`
`flamerhitpush1 5.0`
`flamerhitpush2 10.0`
<span style="color:red; text-decoration:line-through">`flamerjamchance 25`</span><span style="color:green; text-decoration:underline">`flamerinteracts1 1`</span>
<span style="color:green; text-decoration:underline">`flamerinteracts2 1`</span>
`flamerkickpush1 1.0`
`flamerkickpush2 2.0`
`flamerlaser 0`
<span style="color:red; text-decoration:line-through">`flamerlegsdmg1`</span><span style="color:green; text-decoration:underline">`flamerlegdamage1`</span>` 0.25`
<span style="color:red; text-decoration:line-through">`flamerlegsdmg2`</span><span style="color:green; text-decoration:underline">`flamerlegdamage2`</span>` 0.25`
`flamerlimspeed1 0`
`flamerlimspeed2 0`
`flamermax `<span style="color:red; text-decoration:line-through">`25`</span>
<span style="color:red; text-decoration:line-through">`flamermaxspread1 0`</span>
<span style="color:red; text-decoration:line-through">`flamermaxspread2 0`</span><span style="color:green; text-decoration:underline">`30`</span>
`flamerminspeed1 0.0`
`flamerminspeed2 25.0`
<span style="color:red; text-decoration:line-through">`flamerminspread1 0`</span><span style="color:green; text-decoration:underline">`flamermodes -64`</span>
<span style="color:red; text-decoration:line-through">`flamerminspread2 0`</span><span style="color:green; text-decoration:underline">`flamermuts -56`</span>
`flamername "flamer"`
`flamerpartcol1 -1`
`flamerpartcol2 -1`
`flamerpartsize2 10.0`
`flamerparttype1 5`
`flamerparttype2 5`
<span style="color:red; text-decoration:line-through">`flamerpdelay1 0`</span>
<span style="color:red; text-decoration:line-through">`flamerpdelay2 25`</span>
`flamerpower1 0`
`flamerpower2 500`
<span style="color:red; text-decoration:line-through">`flamerpusharea`</span><span style="color:green; text-decoration:underline">`flamerprojdelay1 0`</span>
<span style="color:green; text-decoration:underline">`flamerprojdelay2 25`</span>
<span style="color:green; text-decoration:underline">`flamerproxdelay1 0`</span>
<span style="color:green; text-decoration:underline">`flamerproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`flamerproxdist1 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerproxdist2`</span>` 0.0`
<span style="color:green; text-decoration:underline">`flamerproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`flamerproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`flamerproxtype1 0`</span>
<span style="color:green; text-decoration:underline">`flamerproxtype2 0`</span>
`flamerradial2 `<span style="color:red; text-decoration:line-through">`25`</span><span style="color:green; text-decoration:underline">`20`</span>
`flamerradius1 `<span style="color:red; text-decoration:line-through">`1.0`</span><span style="color:green; text-decoration:underline">`1.5`</span>
`flamerradius2 `<span style="color:red; text-decoration:line-through">`1.0`</span><span style="color:green; text-decoration:underline">`1.5`</span>
`flamerrays1 1`
`flamerrays2 4`
<span style="color:red; text-decoration:line-through">`flamerrdelay 2000`</span>
`flamerreflectivity1 0.0`
`flamerreflectivity2 0.0`
`flamerrelativity1 0.95`
`flamerrelativity2 0.5`
<span style="color:green; text-decoration:underline">`flamerreloaddelay 1750`</span>
`flamerreloads -1`
`flamerresidual1 1`
`flamerresidual2 1`
<span style="color:red; text-decoration:line-through">`flamerselfdmg1 0.5`</span><span style="color:green; text-decoration:underline">`flamerselfdamage1 0.3`</span>
<span style="color:red; text-decoration:line-through">`flamerselfdmg2 0.5`</span>
<span style="color:red; text-decoration:line-through">`flamerslow1 0.0`</span>
<span style="color:red; text-decoration:line-through">`flamerslow2 0.0`</span><span style="color:green; text-decoration:underline">`flamerselfdamage2 0.3`</span>
`flamerspeed1 `<span style="color:red; text-decoration:line-through">`300`</span><span style="color:green; text-decoration:underline">`400`</span>
`flamerspeed2 `<span style="color:red; text-decoration:line-through">`150`</span><span style="color:green; text-decoration:underline">`200`</span>
`flamerspread1 `<span style="color:red; text-decoration:line-through">`5`</span><span style="color:green; text-decoration:underline">`5.0`</span>
`flamerspread2 `<span style="color:red; text-decoration:line-through">`20`</span><span style="color:green; text-decoration:underline">`20.0`</span>
<span style="color:green; text-decoration:underline">`flamerspreadmax1 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerspreadmax2 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerspreadmin1 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerspreadmin2 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerspreadz1 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerspreadz2 1.0`</span>
<span style="color:green; text-decoration:underline">`flamerstunfall1 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerstunfall2 0.0`</span>
`flamerstunscale1 0.0`
`flamerstunscale2 0.0`
`flamerstuntime1 0`
`flamerstuntime2 0`
`flamersub1 1`
`flamersub2 5`
<span style="color:green; text-decoration:underline">`flamertaper1 1`</span>
<span style="color:green; text-decoration:underline">`flamertaper2 1`</span>
`flamertaperin1 0.5`
`flamertaperin2 0.5`
`flamertaperout1 0.0`
`flamertaperout2 0.0`
<span style="color:green; text-decoration:underline">`flamerteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`flamerteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`flamerteampenalty1 1.0`</span>
<span style="color:green; text-decoration:underline">`flamerteampenalty2 1.0`</span>
`flamertime1 200`
`flamertime2 `<span style="color:red; text-decoration:line-through">`1500`</span><span style="color:green; text-decoration:underline">`2000`</span>
<span style="color:red; text-decoration:line-through">`flamertorsodmg1`</span><span style="color:green; text-decoration:underline">`flamertorsodamage1`</span>` 0.45`
<span style="color:red; text-decoration:line-through">`flamertorsodmg2`</span><span style="color:green; text-decoration:underline">`flamertorsodamage2`</span>` 0.45`
`flamertrace1 1.0`
`flamertrace2 1.0`
<span style="color:green; text-decoration:underline">`flamervisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`flamervisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`flamervistime1 0`</span>
<span style="color:green; text-decoration:underline">`flamervistime2 0`</span>
`flamerwaterfric1 1.0`
`flamerwaterfric2 1.0`
<span style="color:green; text-decoration:underline">`flamerwavepush1 0.0`</span>
<span style="color:green; text-decoration:underline">`flamerwavepush2 0.0`</span>
`flamerweight1 200.0`
`flamerweight2 100.0`
<span style="color:red; text-decoration:line-through">`flamerwhipdmg1`</span><span style="color:green; text-decoration:underline">`flamerwhipdamage1`</span>` 0.65`
<span style="color:red; text-decoration:line-through">`flamerwhipdmg2`</span><span style="color:green; text-decoration:underline">`flamerwhipdamage2`</span>` 0.65 `<span style="color:red; text-decoration:line-through">`flamerzdiv1 0`</span>
<span style="color:red; text-decoration:line-through">`flamerzdiv2 1`</span>
`flamerzooms 0`
<span style="color:red; text-decoration:line-through">`floorcoastforce -1.0`</span><span style="color:green; text-decoration:underline">`floodlines 5`</span>
<span style="color:green; text-decoration:underline">`floodlock 4`</span>
<span style="color:green; text-decoration:underline">`floodmute 3`</span>
<span style="color:green; text-decoration:underline">`floodtime 10000`</span>
<span style="color:green; text-decoration:underline">`floorcoast 5.0`</span>
`floorcoastscale 1.0`
`fragbonus 3`
<span style="color:green; text-decoration:underline">`gamepaused 0`</span>
`gamespeed 100`
<span style="color:red; text-decoration:line-through">`gravityforce -1.0`</span><span style="color:green; text-decoration:underline">`gamespeedlock 5`</span>
<span style="color:green; text-decoration:underline">`gauntletbuffarea 256.0`</span>
<span style="color:green; text-decoration:underline">`gauntletbuffdamage 1.5`</span>
<span style="color:green; text-decoration:underline">`gauntletbuffdelay 1000`</span>
<span style="color:green; text-decoration:underline">`gauntletbuffing 1`</span>
<span style="color:green; text-decoration:underline">`gauntletbuffshield 1.5`</span>
<span style="color:green; text-decoration:underline">`gauntletghost 2`</span>
<span style="color:green; text-decoration:underline">`gauntletmaps "ares bath battlefield biolytic canals cargo center colony conflict deli depot dropzone erosion foundation futuresport ghost linear nova stone suspended tribal venus wet"`</span>
<span style="color:green; text-decoration:underline">`gauntletregenbuff 1`</span>
<span style="color:green; text-decoration:underline">`gauntletregendelay 1000`</span>
<span style="color:green; text-decoration:underline">`gauntletregenextra 2`</span>
<span style="color:green; text-decoration:underline">`gauntletweapon 7`</span>
<span style="color:green; text-decoration:underline">`gravity 50.0`</span>
`gravityscale 1.0`
`grenadeadd 1`
<span style="color:red; text-decoration:line-through">`grenadeadelay1 1000`</span>
<span style="color:red; text-decoration:line-through">`grenadeadelay2 1000`</span>
`grenadeaidist1 384.0`
`grenadeaidist2 256.0`
`grenadeaiskew1 5`
`grenadeaiskew2 5`
<span style="color:red; text-decoration:line-through">`grenadeallowed 3`</span><span style="color:green; text-decoration:underline">`grenadeattackdelay1 750`</span>
<span style="color:green; text-decoration:underline">`grenadeattackdelay2 750`</span>
`grenadecarried 0`
`grenadecollide1 `<span style="color:red; text-decoration:line-through">`602`</span><span style="color:green; text-decoration:underline">`230`</span>
`grenadecollide2 `<span style="color:red; text-decoration:line-through">`853`</span><span style="color:green; text-decoration:underline">`12350`</span>
`grenadecolour `<span style="color:red; text-decoration:line-through">`0x119911`</span><span style="color:green; text-decoration:underline">`0x40F000`</span>
`grenadecooked1 8`
`grenadecooked2 8`
<span style="color:red; text-decoration:line-through">`grenadecritdash1 0`</span>
<span style="color:red; text-decoration:line-through">`grenadecritdash2 0`</span>
<span style="color:red; text-decoration:line-through">`grenadecritdist 0.0`</span>
<span style="color:red; text-decoration:line-through">`grenadecritmult 2.0`</span>
`grenadedamage2 `<span style="color:red; text-decoration:line-through">`100`</span><span style="color:green; text-decoration:underline">`150`</span>
`grenadedelta1 10.0`
`grenadedelta2 10.0`
<span style="color:red; text-decoration:line-through">`grenadeedelay1 200`</span><span style="color:green; text-decoration:underline">`grenadedrill1 0`</span>
<span style="color:red; text-decoration:line-through">`grenadeedelay2 200`</span><span style="color:green; text-decoration:underline">`grenadedrill2 0`</span>
`grenadeelasticity1 0.5`
`grenadeelasticity2 0.5`
<span style="color:green; text-decoration:underline">`grenadeescapedelay1 200`</span>
<span style="color:green; text-decoration:underline">`grenadeescapedelay2 200`</span>
`grenadeexplcol1 0x981808`
`grenadeexplcol2 0x981808`
`grenadeexplode1 `<span style="color:red; text-decoration:line-through">`75`</span><span style="color:green; text-decoration:underline">`86.0`</span>
`grenadeexplode2 `<span style="color:red; text-decoration:line-through">`75`</span><span style="color:green; text-decoration:underline">`86.0`</span>
`grenadeextinguish1 2`
`grenadeextinguish2 2`
`grenadeflakcollide1 `<span style="color:red; text-decoration:line-through">`597`</span><span style="color:green; text-decoration:underline">`62`</span>
`grenadeflakcollide2 `<span style="color:red; text-decoration:line-through">`853`</span><span style="color:green; text-decoration:underline">`12350`</span>
<span style="color:red; text-decoration:line-through">`grenadeflakdmg1`</span><span style="color:green; text-decoration:underline">`grenadeflakdamage1`</span>` 150`
<span style="color:red; text-decoration:line-through">`grenadeflakdmg2`</span><span style="color:green; text-decoration:underline">`grenadeflakdamage2`</span>` 150`
<span style="color:red; text-decoration:line-through">`grenadeflakffwd1`</span><span style="color:green; text-decoration:underline">`grenadeflakdelta1 10.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakdelta2 10.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakdrill1 0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakdrill2 0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakelasticity1 0.5`</span>
<span style="color:green; text-decoration:underline">`grenadeflakelasticity2 0.5`</span>
<span style="color:green; text-decoration:underline">`grenadeflakexplcol1 0x981808`</span>
<span style="color:green; text-decoration:underline">`grenadeflakexplcol2 0x981808`</span>
<span style="color:green; text-decoration:underline">`grenadeflakexplode1 86.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakexplode2 86.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakextinguish1 2`</span>
<span style="color:green; text-decoration:underline">`grenadeflakextinguish2 2`</span>
<span style="color:green; text-decoration:underline">`grenadeflakguided1 0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakguided2 0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakguideddelay2 0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakheadmin1 8.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakheadmin2 8.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakhitpush1 250.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakhitpush2 250.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakinteracts1 3`</span>
<span style="color:green; text-decoration:underline">`grenadeflakinteracts2 3`</span>
<span style="color:green; text-decoration:underline">`grenadeflaklegdamage1 0.2`</span>
<span style="color:green; text-decoration:underline">`grenadeflaklegdamage2 0.2`</span>
<span style="color:green; text-decoration:underline">`grenadeflakminspeed1 50.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakminspeed2 50.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakpartcol1 -1`</span>
<span style="color:green; text-decoration:underline">`grenadeflakpartcol2 -1`</span>
<span style="color:green; text-decoration:underline">`grenadeflakpartlen1`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`grenadeflakffwd2`</span><span style="color:green; text-decoration:underline">`grenadeflakpartlen2`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`grenadeflakminspeed1`</span><span style="color:green; text-decoration:underline">`grenadeflakpartsize1 1.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakpartsize2 1.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakparttype1 8`</span>
<span style="color:green; text-decoration:underline">`grenadeflakparttype2 8`</span>
<span style="color:green; text-decoration:underline">`grenadeflakproxdelay1 0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakproxdist1`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`grenadeflakminspeed2`</span><span style="color:green; text-decoration:underline">`grenadeflakproxdist2 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakproxtype1 0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakproxtype2 0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakradial1 0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakradial2 0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakradius1 1.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakradius2 1.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakreflectivity1`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`grenadeflakoffset1`</span><span style="color:green; text-decoration:underline">`grenadeflakreflectivity2`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`grenadeflakoffset2`</span><span style="color:green; text-decoration:underline">`grenadeflakresidual1 1`</span>
<span style="color:green; text-decoration:underline">`grenadeflakresidual2 1`</span>
<span style="color:green; text-decoration:underline">`grenadeflakselfdamage1 0.5`</span>
<span style="color:green; text-decoration:underline">`grenadeflakselfdamage2 0.5`</span>
<span style="color:green; text-decoration:underline">`grenadeflakstunfall1 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakstunfall2 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakstunscale1 2.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakstunscale2 2.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakstuntime1 200`</span>
<span style="color:green; text-decoration:underline">`grenadeflakstuntime2 200`</span>
<span style="color:green; text-decoration:underline">`grenadeflaktaper1 0`</span>
<span style="color:green; text-decoration:underline">`grenadeflaktaper2 0`</span>
<span style="color:green; text-decoration:underline">`grenadeflaktaperin1 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflaktaperin2 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflaktaperout1 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflaktaperout2 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakteampenalty1 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakteampenalty2`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`grenadeflakrays1 75`</span><span style="color:green; text-decoration:underline">`grenadeflaktorsodamage1 0.4`</span>
<span style="color:green; text-decoration:underline">`grenadeflaktorsodamage2 0.4`</span>
<span style="color:green; text-decoration:underline">`grenadeflakvisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakvisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakvistime1 0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakvistime2 0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakwaterfric1 2.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakwaterfric2 2.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakwavepush1 2.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakwavepush2 2.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakweight1 65.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakweight2 65.0`</span>
<span style="color:green; text-decoration:underline">`grenadeflakwhipdamage1 0.6`</span>
<span style="color:green; text-decoration:underline">`grenadeflakwhipdamage2 0.6`</span>
<span style="color:green; text-decoration:underline">`grenadefragdelay1 3`</span>
<span style="color:green; text-decoration:underline">`grenadefragdelay2 3`</span>
<span style="color:green; text-decoration:underline">`grenadefragjump1 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadefragjump2 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadefragoffset1 4.0`</span>
<span style="color:green; text-decoration:underline">`grenadefragoffset2 4.0`</span>
<span style="color:green; text-decoration:underline">`grenadefragrays1 30`</span>
<span style="color:red; text-decoration:line-through">`grenadeflakrays2 75`</span><span style="color:green; text-decoration:underline">`grenadefragrays2 30`</span>
<span style="color:red; text-decoration:line-through">`grenadeflakrel1`</span><span style="color:green; text-decoration:underline">`grenadefragrel1`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`grenadeflakrel2`</span><span style="color:green; text-decoration:underline">`grenadefragrel2`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`grenadeflakscale1`</span><span style="color:green; text-decoration:underline">`grenadefragscale1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`grenadeflakscale2`</span><span style="color:green; text-decoration:underline">`grenadefragscale2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`grenadeflakskew1`</span><span style="color:green; text-decoration:underline">`grenadefragskew1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`grenadeflakskew2`</span><span style="color:green; text-decoration:underline">`grenadefragskew2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`grenadeflakspeed1`</span><span style="color:green; text-decoration:underline">`grenadefragspeed1`</span>` 300`
<span style="color:red; text-decoration:line-through">`grenadeflakspeed2`</span><span style="color:green; text-decoration:underline">`grenadefragspeed2`</span>` 300`
<span style="color:red; text-decoration:line-through">`grenadeflakspread1`</span><span style="color:green; text-decoration:underline">`grenadefragspread1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`grenadeflakspread2`</span><span style="color:green; text-decoration:underline">`grenadefragspread2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`grenadeflaktime1 3000`</span><span style="color:green; text-decoration:underline">`grenadefragtime1 1000`</span>
<span style="color:red; text-decoration:line-through">`grenadeflaktime2 3000`</span><span style="color:green; text-decoration:underline">`grenadefragtime2 1000`</span>
<span style="color:red; text-decoration:line-through">`grenadeflakweap1`</span><span style="color:green; text-decoration:underline">`grenadefragweap1`</span>` 3`
<span style="color:red; text-decoration:line-through">`grenadeflakweap2`</span><span style="color:green; text-decoration:underline">`grenadefragweap2`</span>` 3`
`grenadefrequency 2.0`
`grenadefullauto1 0`
`grenadefullauto2 0`
<span style="color:red; text-decoration:line-through">`grenadegdelay1 0`</span>
<span style="color:red; text-decoration:line-through">`grenadegdelay2 0`</span>
`grenadeguided1 0`
`grenadeguided2 0`
<span style="color:green; text-decoration:underline">`grenadeguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`grenadeguideddelay2 0`</span>
`grenadeheadmin1 8.0`
`grenadeheadmin2 8.0`
`grenadehitpush1 250.0`
`grenadehitpush2 250.0`
<span style="color:red; text-decoration:line-through">`grenadejamchance 50`</span><span style="color:green; text-decoration:underline">`grenadeinteracts1 3`</span>
<span style="color:green; text-decoration:underline">`grenadeinteracts2 3`</span>
`grenadekickpush1 5.0`
`grenadekickpush2 5.0`
`grenadelaser 0`
<span style="color:red; text-decoration:line-through">`grenadelegsdmg1`</span><span style="color:green; text-decoration:underline">`grenadelegdamage1`</span>` 0.2`
<span style="color:red; text-decoration:line-through">`grenadelegsdmg2`</span><span style="color:green; text-decoration:underline">`grenadelegdamage2`</span>` 0.2`
`grenadelimspeed1 0`
`grenadelimspeed2 0`
`grenademax 2`
<span style="color:red; text-decoration:line-through">`grenademaxspread1 0`</span>
<span style="color:red; text-decoration:line-through">`grenademaxspread2 0`</span>
`grenademinspeed1 0.0`
`grenademinspeed2 0.0`
<span style="color:red; text-decoration:line-through">`grenademinspread1 0`</span><span style="color:green; text-decoration:underline">`grenademodes -64`</span>
<span style="color:red; text-decoration:line-through">`grenademinspread2`</span><span style="color:green; text-decoration:underline">`grenademuts`</span>` 0`
`grenadename "grenade"`
`grenadepartcol1 -1`
`grenadepartcol2 -1`
`grenadepartsize2 1.0`
`grenadeparttype1 8`
`grenadeparttype2 8`
<span style="color:red; text-decoration:line-through">`grenadepdelay1 75`</span>
<span style="color:red; text-decoration:line-through">`grenadepdelay2 75`</span>
`grenadepower1 3000`
`grenadepower2 3000`
<span style="color:red; text-decoration:line-through">`grenadepusharea 2.0`</span><span style="color:green; text-decoration:underline">`grenadeprojdelay1 75`</span>
<span style="color:green; text-decoration:underline">`grenadeprojdelay2 75`</span>
<span style="color:green; text-decoration:underline">`grenadeproxdelay1 0`</span>
<span style="color:green; text-decoration:underline">`grenadeproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`grenadeproxdist1 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadeproxdist2 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadeproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`grenadeproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`grenadeproxtype1 0`</span>
<span style="color:green; text-decoration:underline">`grenadeproxtype2 0`</span>
`grenaderadial1 0`
`grenaderadial2 0`
`grenaderadius1 1.0`
`grenaderadius2 1.0`
`grenaderays1 1`
`grenaderays2 1`
<span style="color:red; text-decoration:line-through">`grenaderdelay 1500`</span>
`grenadereflectivity1 0.0`
`grenadereflectivity2 0.0`
`grenaderelativity1 1.0`
`grenaderelativity2 1.0`
<span style="color:green; text-decoration:underline">`grenadereloaddelay 2000`</span>
`grenadereloads 0`
`grenaderesidual1 1`
`grenaderesidual2 1`
<span style="color:red; text-decoration:line-through">`grenadeselfdmg1`</span><span style="color:green; text-decoration:underline">`grenadeselfdamage1`</span>` 0.5`
<span style="color:red; text-decoration:line-through">`grenadeselfdmg2`</span><span style="color:green; text-decoration:underline">`grenadeselfdamage2`</span>` 0.5 `<span style="color:red; text-decoration:line-through">`grenadeslow1 0.0`</span>
<span style="color:red; text-decoration:line-through">`grenadeslow2 0.0`</span>
`grenadespeed1 250`
`grenadespeed2 250`
`grenadespread1 `<span style="color:red; text-decoration:line-through">`1`</span><span style="color:green; text-decoration:underline">`1.0`</span>
`grenadespread2 `<span style="color:red; text-decoration:line-through">`1`</span><span style="color:green; text-decoration:underline">`1.0`</span>
<span style="color:green; text-decoration:underline">`grenadespreadmax1 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadespreadmax2 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadespreadmin1 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadespreadmin2 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadespreadz1 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadespreadz2 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadestunfall1 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadestunfall2 0.0`</span>
`grenadestunscale1 2.0`
`grenadestunscale2 2.0`
`grenadestuntime1 200`
`grenadestuntime2 200`
`grenadesub1 1`
`grenadesub2 1`
<span style="color:green; text-decoration:underline">`grenadetaper1 0`</span>
<span style="color:green; text-decoration:underline">`grenadetaper2 0`</span>
`grenadetaperin1 0.0`
`grenadetaperin2 0.0`
`grenadetaperout1 0.0`
`grenadetaperout2 0.0`
<span style="color:green; text-decoration:underline">`grenadeteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`grenadeteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`grenadeteampenalty1 0.0`</span>
<span style="color:green; text-decoration:underline">`grenadeteampenalty2 0.0`</span>
`grenadetime1 3000`
`grenadetime2 3000`
<span style="color:red; text-decoration:line-through">`grenadetorsodmg1`</span><span style="color:green; text-decoration:underline">`grenadetorsodamage1`</span>` 0.4`
<span style="color:red; text-decoration:line-through">`grenadetorsodmg2`</span><span style="color:green; text-decoration:underline">`grenadetorsodamage2`</span>` 0.4`
`grenadetrace1 1.0`
`grenadetrace2 1.0`
<span style="color:green; text-decoration:underline">`grenadevisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`grenadevisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`grenadevistime1 0`</span>
<span style="color:green; text-decoration:underline">`grenadevistime2 0`</span>
`grenadewaterfric1 2.0`
`grenadewaterfric2 2.0`
<span style="color:green; text-decoration:underline">`grenadewavepush1 2.0`</span>
<span style="color:green; text-decoration:underline">`grenadewavepush2 2.0`</span>
`grenadeweight1 65.0`
`grenadeweight2 65.0`
<span style="color:red; text-decoration:line-through">`grenadewhipdmg1`</span><span style="color:green; text-decoration:underline">`grenadewhipdamage1`</span>` 0.6`
<span style="color:red; text-decoration:line-through">`grenadewhipdmg2`</span><span style="color:green; text-decoration:underline">`grenadewhipdamage2`</span>` 0.6 `<span style="color:red; text-decoration:line-through">`grenadezdiv1 0`</span>
<span style="color:red; text-decoration:line-through">`grenadezdiv2 0`</span>
`grenadezooms 0`
`headshotpoints 1`
`hitpushscale 1.0`
<span style="color:red; text-decoration:line-through">`hitslowscale`</span><span style="color:green; text-decoration:underline">`hitstunscale`</span>` 1.0`
<span style="color:green; text-decoration:underline">`holdmaps "ares bath battlefield biolytic canals cargo center colony conflict cutec darkness deadsimple deli depot dropzone dutility echo erosion foundation fourplex futuresport ghost keystone2k linear mist nova panic processing pumpstation stone suspended tower tribal ubik vault venus warp wet"`</span>
`impulseallowed 15`
`impulseboost 1.0`
`impulsecost `<span style="color:red; text-decoration:line-through">`4000`</span><span style="color:green; text-decoration:underline">`5000`</span>
<span style="color:green; text-decoration:underline">`impulsecostrelax 8`</span>
`impulsecostscale 0`
`impulsecount 6`
`impulsedash 1.2`
`impulsedashdelay `<span style="color:red; text-decoration:line-through">`750`</span><span style="color:green; text-decoration:underline">`1000`</span>
`impulsedelay 250`
`impulsejet 0.5`
`impulsejump 1.1`
`impulsekickdelay 350`
`impulselimit 0.0`
`impulsemelee 0.75`
<span style="color:green; text-decoration:underline">`impulsepacing 0.0`</span>
`impulseparkour 1.0`
`impulseparkourkick 1.3`
`impulseparkournorm 0.5`
`impulseparkourvault 1.3`
`impulsepower 1.5`
`impulseregen `<span style="color:red; text-decoration:line-through">`4.0`</span><span style="color:green; text-decoration:underline">`5.0`</span>
`impulseregencrouch `<span style="color:red; text-decoration:line-through">`2.0`</span><span style="color:green; text-decoration:underline">`2.5`</span>
`impulseregendelay `<span style="color:red; text-decoration:line-through">`250`</span><span style="color:green; text-decoration:underline">`350`</span>
`impulseregeninair 0.75`
`impulseregenjet `<span style="color:red; text-decoration:line-through">`1.5`</span><span style="color:green; text-decoration:underline">`2.0`</span>
`impulseregenjetdelay -1`
`impulseregenmove 1.0`
<span style="color:red; text-decoration:line-through">`impulseregensprint`</span><span style="color:green; text-decoration:underline">`impulseregenpacing`</span>` 0.75`
<span style="color:green; text-decoration:underline">`impulseregenslide 0.0`</span>
`impulseskate 1000`
`impulseslide `<span style="color:red; text-decoration:line-through">`750`</span><span style="color:green; text-decoration:underline">`1000`</span>
`impulseslip `<span style="color:red; text-decoration:line-through">`350`</span><span style="color:green; text-decoration:underline">`250`</span>
`impulsespeed 90.0`
`impulsespread 1.0`
<span style="color:red; text-decoration:line-through">`impulsesprint 0.0`</span>
`impulsestyle 1`
`impulsevaultmax 1.0`
`impulsevaultmin 0.25`
`inairspread `<span style="color:red; text-decoration:line-through">`1.0`</span><span style="color:green; text-decoration:underline">`2.0`</span>
`instadelay 3000`
`instaprotect 3000`
`instaresizeamt 0.1`
`instaweapon 7`
`intermlimit 15000`
`itemcollide `<span style="color:red; text-decoration:line-through">`2`</span><span style="color:green; text-decoration:underline">`64`</span>
`itemelasticity 0.4`
`itemextinguish 6`
<span style="color:green; text-decoration:underline">`iteminteracts 3`</span>
`itemminspeed 0.0`
`itemrelativity 1.0`
`itemrepelspeed 25.0`
`jetdecay 15.0`
`jetdelay 250`
`jetheight 0.0`
<span style="color:green; text-decoration:underline">`jetpackmaps "ares battlefield biolytic canals cargo center colony conflict cutec darkness deadsimple deathtrap deli depot dropzone dutility echo erosion error forge fourplex futuresport ghost linear longestyard mist nova oneiroi pumpstation spacetech starlibido suspended testchamber tower tranquility tribal ubik venus warp"`</span>
`jumpspeed 110.0`
`kamikaze 1`
<span style="color:green; text-decoration:underline">`kicklock 3`</span>
`kickpushcrouch 0.0`
`kickpushscale 1.0`
`kickpushsway 0.0125`
`kickpushzoom 0.125`
<span style="color:red; text-decoration:line-through">`liquidcoastforce -1.0`</span><span style="color:green; text-decoration:underline">`kingmaps "ares bath battlefield biolytic canals cargo center colony conflict darkness deadsimple depot dutility echo fourplex linear livefire processing stone suspended tower tribal ubik vault venus"`</span>
<span style="color:green; text-decoration:underline">`largemaps "ares battlefield biolytic canals cargo center colony cutec deadsimple deathtrap deli depot erosion forge foundation futuresport ghost linear mist nova processing pumpstation spacetech suspended tower tranquility tribal ubik venus warp"`</span>
<span style="color:green; text-decoration:underline">`limitlock 3`</span>
<span style="color:green; text-decoration:underline">`liquidcoast 10.0`</span>
`liquidcoastscale 1.0`
<span style="color:red; text-decoration:line-through">`liquidspeedforce -1.0`</span><span style="color:green; text-decoration:underline">`liquidextinguish 0.25`</span>
<span style="color:green; text-decoration:underline">`liquidextinguishscale 1.0`</span>
<span style="color:green; text-decoration:underline">`liquidspeed 0.85`</span>
`liquidspeedscale 1.0`
<span style="color:green; text-decoration:underline">`liquidsubmerge 0.75`</span>
<span style="color:green; text-decoration:underline">`liquidsubmergescale 1.0`</span>
<span style="color:green; text-decoration:underline">`mainmaps "ares bath battlefield biolytic bloodlust canals cargo center colony conflict cutec darkness deadsimple deathtrap deli depot dropzone dutility echo erosion error foundation fourplex futuresport ghost institute keystone2k linear livefire longestyard mist nova oneiroi panic processing pumpstation spacetech starlibido stone suspended tower tribal ubik vault venus warp wet"`</span>
<span style="color:green; text-decoration:underline">`mapbalance 0`</span>
<span style="color:green; text-decoration:underline">`maphistory 5`</span>
<span style="color:green; text-decoration:underline">`mapsfilter 1`</span>
<span style="color:green; text-decoration:underline">`mapslock 4`</span>
<span style="color:green; text-decoration:underline">`mapslocktype 2`</span>
<span style="color:green; text-decoration:underline">`masterlock 3`</span>
`maxaliveminimum `<span style="color:red; text-decoration:line-through">`8`</span><span style="color:green; text-decoration:underline">`4`</span>
`maxalivequeue 1`
`maxalivethreshold `<span style="color:red; text-decoration:line-through">`0.5`</span><span style="color:green; text-decoration:underline">`0.0`</span>
`maxcarry 2`
`maxhealth 1.5`
`maxhealthvampire 2.0`
<span style="color:green; text-decoration:underline">`maxplayers 0`</span>
`maxresizescale 2.0`
<span style="color:green; text-decoration:underline">`mediummapmax 12`</span>
<span style="color:green; text-decoration:underline">`mediummaps "ares battlefield biolytic canals cargo center colony conflict cutec darkness deadsimple deathtrap deli dropzone echo erosion error forge foundation fourplex futuresport ghost institute keystone2k linear livefire mist nova oneiroi panic processing pumpstation spacetech suspended starlibido stone tower tranquility tribal ubik venus warp wet"`</span>
`meleeadd 1`
<span style="color:red; text-decoration:line-through">`meleeadelay1 250`</span>
<span style="color:red; text-decoration:line-through">`meleeadelay2 500`</span>
`meleeaidist1 16.0`
`meleeaidist2 16.0`
`meleeaiskew1 1`
`meleeaiskew2 1`
<span style="color:red; text-decoration:line-through">`meleeallowed 2`</span><span style="color:green; text-decoration:underline">`meleeattackdelay1 500`</span>
<span style="color:green; text-decoration:underline">`meleeattackdelay2 1000`</span>
`meleecarried 0`
`meleecollide1 `<span style="color:red; text-decoration:line-through">`36`</span><span style="color:green; text-decoration:underline">`17`</span>
`meleecollide2 `<span style="color:red; text-decoration:line-through">`36`</span><span style="color:green; text-decoration:underline">`17`</span>
`meleecolour `<span style="color:red; text-decoration:line-through">`0xEEEEEE`</span><span style="color:green; text-decoration:underline">`0x707070`</span>
`meleecooked1 0`
`meleecooked2 0`
<span style="color:red; text-decoration:line-through">`meleecritboost 2.0`</span>
<span style="color:red; text-decoration:line-through">`meleecritdash1 500`</span>
<span style="color:red; text-decoration:line-through">`meleecritdash2 500`</span>
<span style="color:red; text-decoration:line-through">`meleecritdist 0.0`</span>
<span style="color:red; text-decoration:line-through">`meleecritmult 2.0`</span>
`meleedamage1 30`
`meleedamage2 40`
`meleedelta1 10.0`
`meleedelta2 10.0`
<span style="color:red; text-decoration:line-through">`meleeedelay1 200`</span><span style="color:green; text-decoration:underline">`meleedrill1 0`</span>
<span style="color:red; text-decoration:line-through">`meleeedelay2 200`</span><span style="color:green; text-decoration:underline">`meleedrill2 0`</span>
`meleeelasticity1 0.5`
`meleeelasticity2 0.5`
<span style="color:green; text-decoration:underline">`meleeescapedelay1 200`</span>
<span style="color:green; text-decoration:underline">`meleeescapedelay2 200`</span>
`meleeexplcol1 -1`
`meleeexplcol2 -1`
`meleeexplode1 `<span style="color:red; text-decoration:line-through">`0`</span><span style="color:green; text-decoration:underline">`0.0`</span>
`meleeexplode2 `<span style="color:red; text-decoration:line-through">`0`</span><span style="color:green; text-decoration:underline">`0.0`</span>
`meleeextinguish1 2`
`meleeextinguish2 2`
`meleeflakcollide1 `<span style="color:red; text-decoration:line-through">`36`</span><span style="color:green; text-decoration:underline">`21`</span>
`meleeflakcollide2 `<span style="color:red; text-decoration:line-through">`36`</span><span style="color:green; text-decoration:underline">`21`</span>
<span style="color:red; text-decoration:line-through">`meleeflakdmg1`</span><span style="color:green; text-decoration:underline">`meleeflakdamage1`</span>` 25`
<span style="color:red; text-decoration:line-through">`meleeflakdmg2`</span><span style="color:green; text-decoration:underline">`meleeflakdamage2`</span>` 10`
<span style="color:red; text-decoration:line-through">`meleeflakffwd1`</span><span style="color:green; text-decoration:underline">`meleeflakdelta1 10.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakdelta2 10.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakdrill1 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakdrill2 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakelasticity1 0.5`</span>
<span style="color:green; text-decoration:underline">`meleeflakelasticity2 0.5`</span>
<span style="color:green; text-decoration:underline">`meleeflakexplcol1 -1`</span>
<span style="color:green; text-decoration:underline">`meleeflakexplcol2 -1`</span>
<span style="color:green; text-decoration:underline">`meleeflakexplode1`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`meleeflakffwd2`</span><span style="color:green; text-decoration:underline">`meleeflakexplode2`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`meleeflakminspeed1`</span><span style="color:green; text-decoration:underline">`meleeflakextinguish1 2`</span>
<span style="color:green; text-decoration:underline">`meleeflakextinguish2 2`</span>
<span style="color:green; text-decoration:underline">`meleeflakguided1 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakguided2 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakguideddelay2 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakheadmin1`</span>` 0.0`
<span style="color:green; text-decoration:underline">`meleeflakheadmin2 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakhitpush1 100.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakhitpush2 200.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakinteracts1 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakinteracts2 0`</span>
<span style="color:green; text-decoration:underline">`meleeflaklegdamage1 0.3`</span>
<span style="color:green; text-decoration:underline">`meleeflaklegdamage2 0.6`</span>
<span style="color:green; text-decoration:underline">`meleeflakminspeed1 50.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakpartcol1 0xEEEE22`</span>
<span style="color:green; text-decoration:underline">`meleeflakpartcol2 0xEEEE22`</span>
<span style="color:green; text-decoration:underline">`meleeflakpartlen1 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakpartlen2 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakpartsize1 1.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakpartsize2 2.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakparttype1 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakparttype2 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakproxdelay1 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakproxdist1 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakproxdist2 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakproxtype1 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakproxtype2 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakradial1 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakradial2 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakradius1 1.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakradius2 1.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakreflectivity1 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakreflectivity2 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakresidual1 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakresidual2 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakselfdamage1 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakselfdamage2 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakstunfall1 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakstunfall2 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakstunscale1 0.5`</span>
<span style="color:green; text-decoration:underline">`meleeflakstunscale2 1.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakstuntime1 100`</span>
<span style="color:green; text-decoration:underline">`meleeflakstuntime2 200`</span>
<span style="color:green; text-decoration:underline">`meleeflaktaper1 0`</span>
<span style="color:green; text-decoration:underline">`meleeflaktaper2 0`</span>
<span style="color:green; text-decoration:underline">`meleeflaktaperin1 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeflaktaperin2 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeflaktaperout1 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeflaktaperout2 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakteampenalty1 1.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakteampenalty2 1.0`</span>
<span style="color:green; text-decoration:underline">`meleeflaktorsodamage1 0.5`</span>
<span style="color:green; text-decoration:underline">`meleeflaktorsodamage2 0.8`</span>
<span style="color:green; text-decoration:underline">`meleeflakvisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakvisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakvistime1 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakvistime2 0`</span>
<span style="color:green; text-decoration:underline">`meleeflakwaterfric1 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakwaterfric2 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakwavepush1 1.5`</span>
<span style="color:green; text-decoration:underline">`meleeflakwavepush2 1.5`</span>
<span style="color:green; text-decoration:underline">`meleeflakweight1 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakweight2 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeflakwhipdamage1 0.8`</span>
<span style="color:green; text-decoration:underline">`meleeflakwhipdamage2 0.8`</span>
<span style="color:green; text-decoration:underline">`meleefragdelay1 0`</span>
<span style="color:green; text-decoration:underline">`meleefragdelay2 0`</span>
<span style="color:green; text-decoration:underline">`meleefragjump1 0.0`</span>
<span style="color:green; text-decoration:underline">`meleefragjump2`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`meleeflakoffset1 8.0`</span><span style="color:green; text-decoration:underline">`meleefragoffset1 4.0`</span>
<span style="color:red; text-decoration:line-through">`meleeflakoffset2 8.0`</span><span style="color:green; text-decoration:underline">`meleefragoffset2 4.0`</span>
<span style="color:red; text-decoration:line-through">`meleeflakrays1`</span><span style="color:green; text-decoration:underline">`meleefragrays1`</span>` 5`
<span style="color:red; text-decoration:line-through">`meleeflakrays2`</span><span style="color:green; text-decoration:underline">`meleefragrays2`</span>` 5`
<span style="color:red; text-decoration:line-through">`meleeflakrel1`</span><span style="color:green; text-decoration:underline">`meleefragrel1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`meleeflakrel2`</span><span style="color:green; text-decoration:underline">`meleefragrel2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`meleeflakscale1`</span><span style="color:green; text-decoration:underline">`meleefragscale1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`meleeflakscale2`</span><span style="color:green; text-decoration:underline">`meleefragscale2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`meleeflakskew1`</span><span style="color:green; text-decoration:underline">`meleefragskew1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`meleeflakskew2`</span><span style="color:green; text-decoration:underline">`meleefragskew2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`meleeflakspeed1`</span><span style="color:green; text-decoration:underline">`meleefragspeed1`</span>` 0`
<span style="color:red; text-decoration:line-through">`meleeflakspeed2`</span><span style="color:green; text-decoration:underline">`meleefragspeed2`</span>` 0`
<span style="color:red; text-decoration:line-through">`meleeflakspread1`</span><span style="color:green; text-decoration:underline">`meleefragspread1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`meleeflakspread2`</span><span style="color:green; text-decoration:underline">`meleefragspread2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`meleeflaktime1`</span><span style="color:green; text-decoration:underline">`meleefragtime1`</span>` 500`
<span style="color:red; text-decoration:line-through">`meleeflaktime2`</span><span style="color:green; text-decoration:underline">`meleefragtime2`</span>` 500`
<span style="color:red; text-decoration:line-through">`meleeflakweap1`</span><span style="color:green; text-decoration:underline">`meleefragweap1`</span>` -1`
<span style="color:red; text-decoration:line-through">`meleeflakweap2`</span><span style="color:green; text-decoration:underline">`meleefragweap2`</span>` -1`
`meleefrequency 0.0`
`meleefullauto1 1`
`meleefullauto2 1`
<span style="color:red; text-decoration:line-through">`meleegdelay1 0`</span>
<span style="color:red; text-decoration:line-through">`meleegdelay2 0`</span>
`meleeguided1 0`
`meleeguided2 0`
<span style="color:green; text-decoration:underline">`meleeguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`meleeguideddelay2 0`</span>
`meleeheadmin1 0.0`
`meleeheadmin2 0.0`
`meleehitpush1 `<span style="color:red; text-decoration:line-through">`50.0`</span><span style="color:green; text-decoration:underline">`100.0`</span>
`meleehitpush2 `<span style="color:red; text-decoration:line-through">`100.0`</span><span style="color:green; text-decoration:underline">`200.0`</span>
<span style="color:green; text-decoration:underline">`meleeinteracts1 0`</span>
<span style="color:red; text-decoration:line-through">`meleejamchance`</span><span style="color:green; text-decoration:underline">`meleeinteracts2`</span>` 0`
`meleekickpush1 0.0`
`meleekickpush2 0.0`
`meleelaser 0`
<span style="color:red; text-decoration:line-through">`meleelegsdmg1`</span><span style="color:green; text-decoration:underline">`meleelegdamage1`</span>` 0.3`
<span style="color:red; text-decoration:line-through">`meleelegsdmg2 0.3`</span><span style="color:green; text-decoration:underline">`meleelegdamage2 0.6`</span>
`meleelimspeed1 0`
`meleelimspeed2 0`
`meleemax 1`
<span style="color:red; text-decoration:line-through">`meleemaxspread1 0`</span>
<span style="color:red; text-decoration:line-through">`meleemaxspread2 0`</span>
`meleeminspeed1 0.0`
`meleeminspeed2 0.0`
<span style="color:red; text-decoration:line-through">`meleeminspread1`</span><span style="color:green; text-decoration:underline">`meleemodes`</span>` 0`
<span style="color:red; text-decoration:line-through">`meleeminspread2`</span><span style="color:green; text-decoration:underline">`meleemuts`</span>` 0`
`meleename "melee"`
`meleepartcol1 0xEEEE22`
`meleepartcol2 0xEEEE22`
`meleepartsize2 2.0`
`meleeparttype1 0`
`meleeparttype2 0`
<span style="color:red; text-decoration:line-through">`meleepdelay1 10`</span>
<span style="color:red; text-decoration:line-through">`meleepdelay2 10`</span>
`meleepower1 0`
`meleepower2 0`
<span style="color:red; text-decoration:line-through">`meleepusharea 1.0`</span><span style="color:green; text-decoration:underline">`meleeprojdelay1 0`</span>
<span style="color:green; text-decoration:underline">`meleeprojdelay2 0`</span>
<span style="color:green; text-decoration:underline">`meleeproxdelay1 0`</span>
<span style="color:green; text-decoration:underline">`meleeproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`meleeproxdist1 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeproxdist2 0.0`</span>
<span style="color:green; text-decoration:underline">`meleeproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`meleeproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`meleeproxtype1 0`</span>
<span style="color:green; text-decoration:underline">`meleeproxtype2 0`</span>
`meleeradial1 0`
`meleeradial2 0`
`meleeradius1 1.0`
`meleeradius2 1.0`
`meleerays1 1`
`meleerays2 1`
<span style="color:red; text-decoration:line-through">`meleerdelay 50`</span>
`meleereflectivity1 0.0`
`meleereflectivity2 0.0`
`meleerelativity1 0.0`
`meleerelativity2 0.0`
<span style="color:green; text-decoration:underline">`meleereloaddelay 50`</span>
`meleeresidual1 0`
`meleeresidual2 0`
<span style="color:red; text-decoration:line-through">`meleeselfdmg1`</span><span style="color:green; text-decoration:underline">`meleeselfdamage1`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`meleeselfdmg2 0.0`</span>
<span style="color:red; text-decoration:line-through">`meleeslow1 0.0`</span>
<span style="color:red; text-decoration:line-through">`meleeslow2`</span><span style="color:green; text-decoration:underline">`meleeselfdamage2`</span>` 0.0`
`meleespeed1 0`
`meleespeed2 0`
`meleespread1 `<span style="color:red; text-decoration:line-through">`1`</span><span style="color:green; text-decoration:underline">`1.0`</span>
`meleespread2 `<span style="color:red; text-decoration:line-through">`1`</span><span style="color:green; text-decoration:underline">`1.0`</span>
<span style="color:green; text-decoration:underline">`meleespreadmax1 0.0`</span>
<span style="color:green; text-decoration:underline">`meleespreadmax2 0.0`</span>
<span style="color:green; text-decoration:underline">`meleespreadmin1 0.0`</span>
<span style="color:green; text-decoration:underline">`meleespreadmin2 0.0`</span>
<span style="color:green; text-decoration:underline">`meleespreadz1 1.0`</span>
<span style="color:green; text-decoration:underline">`meleespreadz2 1.0`</span>
<span style="color:green; text-decoration:underline">`meleestunfall1 0.0`</span>
<span style="color:green; text-decoration:underline">`meleestunfall2 0.0`</span>
`meleestunscale1 0.5`
`meleestunscale2 `<span style="color:red; text-decoration:line-through">`0.5`</span><span style="color:green; text-decoration:underline">`1.0`</span>
`meleestuntime1 `<span style="color:red; text-decoration:line-through">`50`</span><span style="color:green; text-decoration:underline">`100`</span>
`meleestuntime2 `<span style="color:red; text-decoration:line-through">`100`</span><span style="color:green; text-decoration:underline">`200`</span>
`meleesub1 0`
`meleesub2 0`
<span style="color:green; text-decoration:underline">`meleetaper1 0`</span>
<span style="color:green; text-decoration:underline">`meleetaper2 0`</span>
`meleetaperin1 0.0`
`meleetaperin2 0.0`
`meleetaperout1 0.0`
`meleetaperout2 0.0`
<span style="color:green; text-decoration:underline">`meleeteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`meleeteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`meleeteampenalty1 1.0`</span>
<span style="color:green; text-decoration:underline">`meleeteampenalty2 1.0`</span>
`meleetime1 100`
`meleetime2 `<span style="color:red; text-decoration:line-through">`100`</span><span style="color:green; text-decoration:underline">`350`</span>
<span style="color:red; text-decoration:line-through">`meleetorsodmg1 0.7`</span><span style="color:green; text-decoration:underline">`meleetorsodamage1 0.5`</span>
<span style="color:red; text-decoration:line-through">`meleetorsodmg2 0.6`</span><span style="color:green; text-decoration:underline">`meleetorsodamage2 0.8`</span>
`meleetrace1 `<span style="color:red; text-decoration:line-through">`4.0`</span><span style="color:green; text-decoration:underline">`2.0`</span>
`meleetrace2 `<span style="color:red; text-decoration:line-through">`4.0`</span><span style="color:green; text-decoration:underline">`2.0`</span>
<span style="color:green; text-decoration:underline">`meleevisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`meleevisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`meleevistime1 0`</span>
<span style="color:green; text-decoration:underline">`meleevistime2 0`</span>
`meleewaterfric1 0.0`
`meleewaterfric2 0.0`
<span style="color:green; text-decoration:underline">`meleewavepush1 1.5`</span>
<span style="color:green; text-decoration:underline">`meleewavepush2 1.5`</span>
`meleeweight1 0.0`
`meleeweight2 0.0`
<span style="color:red; text-decoration:line-through">`meleewhipdmg1`</span><span style="color:green; text-decoration:underline">`meleewhipdamage1`</span>` 0.8`
<span style="color:red; text-decoration:line-through">`meleewhipdmg2`</span><span style="color:green; text-decoration:underline">`meleewhipdamage2`</span>` 0.8 `<span style="color:red; text-decoration:line-through">`meleezdiv1 1`</span>
<span style="color:red; text-decoration:line-through">`meleezdiv2 1`</span>
`meleezooms 0`
<span style="color:green; text-decoration:underline">`messagelength 128`</span>
<span style="color:green; text-decoration:underline">`messagelock 0`</span>
<span style="color:green; text-decoration:underline">`mineadd 1`</span>
<span style="color:green; text-decoration:underline">`mineaidist1 128.0`</span>
<span style="color:green; text-decoration:underline">`mineaidist2 128.0`</span>
<span style="color:green; text-decoration:underline">`mineaiskew1 5`</span>
<span style="color:green; text-decoration:underline">`mineaiskew2 5`</span>
<span style="color:green; text-decoration:underline">`mineattackdelay1 1000`</span>
<span style="color:green; text-decoration:underline">`mineattackdelay2 1000`</span>
<span style="color:green; text-decoration:underline">`minecarried 0`</span>
<span style="color:green; text-decoration:underline">`minecollide1 12350`</span>
<span style="color:green; text-decoration:underline">`minecollide2 12350`</span>
<span style="color:green; text-decoration:underline">`minecolour 0x00F068`</span>
<span style="color:green; text-decoration:underline">`minecooked1 8`</span>
<span style="color:green; text-decoration:underline">`minecooked2 8`</span>
<span style="color:green; text-decoration:underline">`minedamage1 150`</span>
<span style="color:green; text-decoration:underline">`minedamage2 150`</span>
<span style="color:green; text-decoration:underline">`minedelta1 10.0`</span>
<span style="color:green; text-decoration:underline">`minedelta2 10.0`</span>
<span style="color:green; text-decoration:underline">`minedrill1 0`</span>
<span style="color:green; text-decoration:underline">`minedrill2 0`</span>
<span style="color:green; text-decoration:underline">`mineelasticity1 0.5`</span>
<span style="color:green; text-decoration:underline">`mineelasticity2 0.5`</span>
<span style="color:green; text-decoration:underline">`mineescapedelay1 200`</span>
<span style="color:green; text-decoration:underline">`mineescapedelay2 200`</span>
<span style="color:green; text-decoration:underline">`mineexplcol1 0x00F068`</span>
<span style="color:green; text-decoration:underline">`mineexplcol2 0x00F068`</span>
<span style="color:green; text-decoration:underline">`mineexplode1 32.0`</span>
<span style="color:green; text-decoration:underline">`mineexplode2 32.0`</span>
<span style="color:green; text-decoration:underline">`mineextinguish1 2`</span>
<span style="color:green; text-decoration:underline">`mineextinguish2 2`</span>
<span style="color:green; text-decoration:underline">`mineflakcollide1 12350`</span>
<span style="color:green; text-decoration:underline">`mineflakcollide2 12350`</span>
<span style="color:green; text-decoration:underline">`mineflakdamage1 150`</span>
<span style="color:green; text-decoration:underline">`mineflakdamage2 150`</span>
<span style="color:green; text-decoration:underline">`mineflakdelta1 10.0`</span>
<span style="color:green; text-decoration:underline">`mineflakdelta2 10.0`</span>
<span style="color:green; text-decoration:underline">`mineflakdrill1 0`</span>
<span style="color:green; text-decoration:underline">`mineflakdrill2 0`</span>
<span style="color:green; text-decoration:underline">`mineflakelasticity1 0.5`</span>
<span style="color:green; text-decoration:underline">`mineflakelasticity2 0.5`</span>
<span style="color:green; text-decoration:underline">`mineflakexplcol1 0x00F068`</span>
<span style="color:green; text-decoration:underline">`mineflakexplcol2 0x00F068`</span>
<span style="color:green; text-decoration:underline">`mineflakexplode1 32.0`</span>
<span style="color:green; text-decoration:underline">`mineflakexplode2 32.0`</span>
<span style="color:green; text-decoration:underline">`mineflakextinguish1 2`</span>
<span style="color:green; text-decoration:underline">`mineflakextinguish2 2`</span>
<span style="color:green; text-decoration:underline">`mineflakguided1 0`</span>
<span style="color:green; text-decoration:underline">`mineflakguided2 0`</span>
<span style="color:green; text-decoration:underline">`mineflakguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`mineflakguideddelay2 0`</span>
<span style="color:green; text-decoration:underline">`mineflakheadmin1 8.0`</span>
<span style="color:green; text-decoration:underline">`mineflakheadmin2 8.0`</span>
<span style="color:green; text-decoration:underline">`mineflakhitpush1 0.0`</span>
<span style="color:green; text-decoration:underline">`mineflakhitpush2 0.0`</span>
<span style="color:green; text-decoration:underline">`mineflakinteracts1 3`</span>
<span style="color:green; text-decoration:underline">`mineflakinteracts2 3`</span>
<span style="color:green; text-decoration:underline">`mineflaklegdamage1 0.2`</span>
<span style="color:green; text-decoration:underline">`mineflaklegdamage2 0.2`</span>
<span style="color:green; text-decoration:underline">`mineflakminspeed1 50.0`</span>
<span style="color:green; text-decoration:underline">`mineflakminspeed2 50.0`</span>
<span style="color:green; text-decoration:underline">`mineflakpartcol1 0x00F068`</span>
<span style="color:green; text-decoration:underline">`mineflakpartcol2 0x00F068`</span>
<span style="color:green; text-decoration:underline">`mineflakpartlen1 4.0`</span>
<span style="color:green; text-decoration:underline">`mineflakpartlen2 4.0`</span>
<span style="color:green; text-decoration:underline">`mineflakpartsize1 2.0`</span>
<span style="color:green; text-decoration:underline">`mineflakpartsize2 2.0`</span>
<span style="color:green; text-decoration:underline">`mineflakparttype1 9`</span>
<span style="color:green; text-decoration:underline">`mineflakparttype2 9`</span>
<span style="color:green; text-decoration:underline">`mineflakproxdelay1 3000`</span>
<span style="color:green; text-decoration:underline">`mineflakproxdelay2 1500000`</span>
<span style="color:green; text-decoration:underline">`mineflakproxdist1 32.0`</span>
<span style="color:green; text-decoration:underline">`mineflakproxdist2 1000000.0`</span>
<span style="color:green; text-decoration:underline">`mineflakproxtime1 100`</span>
<span style="color:green; text-decoration:underline">`mineflakproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`mineflakproxtype1 1`</span>
<span style="color:green; text-decoration:underline">`mineflakproxtype2 2`</span>
<span style="color:green; text-decoration:underline">`mineflakradial1 0`</span>
<span style="color:green; text-decoration:underline">`mineflakradial2 0`</span>
<span style="color:green; text-decoration:underline">`mineflakradius1 1.0`</span>
<span style="color:green; text-decoration:underline">`mineflakradius2 1.0`</span>
<span style="color:green; text-decoration:underline">`mineflakreflectivity1 0.0`</span>
<span style="color:green; text-decoration:underline">`mineflakreflectivity2 0.0`</span>
<span style="color:green; text-decoration:underline">`mineflakresidual1 4`</span>
<span style="color:green; text-decoration:underline">`mineflakresidual2 4`</span>
<span style="color:green; text-decoration:underline">`mineflakselfdamage1 0.5`</span>
<span style="color:green; text-decoration:underline">`mineflakselfdamage2 0.5`</span>
<span style="color:green; text-decoration:underline">`mineflakstunfall1 8.0`</span>
<span style="color:green; text-decoration:underline">`mineflakstunfall2 16.0`</span>
<span style="color:green; text-decoration:underline">`mineflakstunscale1 8.0`</span>
<span style="color:green; text-decoration:underline">`mineflakstunscale2 16.0`</span>
<span style="color:green; text-decoration:underline">`mineflakstuntime1 500`</span>
<span style="color:green; text-decoration:underline">`mineflakstuntime2 750`</span>
<span style="color:green; text-decoration:underline">`mineflaktaper1 0`</span>
<span style="color:green; text-decoration:underline">`mineflaktaper2 0`</span>
<span style="color:green; text-decoration:underline">`mineflaktaperin1 0.0`</span>
<span style="color:green; text-decoration:underline">`mineflaktaperin2 0.0`</span>
<span style="color:green; text-decoration:underline">`mineflaktaperout1 0.0`</span>
<span style="color:green; text-decoration:underline">`mineflaktaperout2 0.0`</span>
<span style="color:green; text-decoration:underline">`mineflakteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`mineflakteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`mineflakteampenalty1 0.0`</span>
<span style="color:green; text-decoration:underline">`mineflakteampenalty2 0.0`</span>
<span style="color:green; text-decoration:underline">`mineflaktorsodamage1 0.4`</span>
<span style="color:green; text-decoration:underline">`mineflaktorsodamage2 0.4`</span>
<span style="color:green; text-decoration:underline">`mineflakvisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`mineflakvisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`mineflakvistime1 0`</span>
<span style="color:green; text-decoration:underline">`mineflakvistime2 0`</span>
<span style="color:green; text-decoration:underline">`mineflakwaterfric1 2.0`</span>
<span style="color:green; text-decoration:underline">`mineflakwaterfric2 2.0`</span>
<span style="color:green; text-decoration:underline">`mineflakwavepush1 2.0`</span>
<span style="color:green; text-decoration:underline">`mineflakwavepush2 2.0`</span>
<span style="color:green; text-decoration:underline">`mineflakweight1 150.0`</span>
<span style="color:green; text-decoration:underline">`mineflakweight2 150.0`</span>
<span style="color:green; text-decoration:underline">`mineflakwhipdamage1 0.6`</span>
<span style="color:green; text-decoration:underline">`mineflakwhipdamage2 0.6`</span>
<span style="color:green; text-decoration:underline">`minefragdelay1 5`</span>
<span style="color:green; text-decoration:underline">`minefragdelay2 100`</span>
<span style="color:green; text-decoration:underline">`minefragjump1 0.0`</span>
<span style="color:green; text-decoration:underline">`minefragjump2 0.0`</span>
<span style="color:green; text-decoration:underline">`minefragoffset1 1.0`</span>
<span style="color:green; text-decoration:underline">`minefragoffset2 1.0`</span>
<span style="color:green; text-decoration:underline">`minefragrays1 30`</span>
<span style="color:green; text-decoration:underline">`minefragrays2 10`</span>
<span style="color:green; text-decoration:underline">`minefragrel1 0.0`</span>
<span style="color:green; text-decoration:underline">`minefragrel2 0.0`</span>
<span style="color:green; text-decoration:underline">`minefragscale1 1.0`</span>
<span style="color:green; text-decoration:underline">`minefragscale2 1.0`</span>
<span style="color:green; text-decoration:underline">`minefragskew1 0.5`</span>
<span style="color:green; text-decoration:underline">`minefragskew2 0.0`</span>
<span style="color:green; text-decoration:underline">`minefragspeed1 750`</span>
<span style="color:green; text-decoration:underline">`minefragspeed2 7500`</span>
<span style="color:green; text-decoration:underline">`minefragspread1 0.5`</span>
<span style="color:green; text-decoration:underline">`minefragspread2 0.1`</span>
<span style="color:green; text-decoration:underline">`minefragtime1 1000`</span>
<span style="color:green; text-decoration:underline">`minefragtime2 5000`</span>
<span style="color:green; text-decoration:underline">`minefragweap1 7`</span>
<span style="color:green; text-decoration:underline">`minefragweap2 18`</span>
<span style="color:green; text-decoration:underline">`minefrequency 2.0`</span>
<span style="color:green; text-decoration:underline">`minefullauto1 0`</span>
<span style="color:green; text-decoration:underline">`minefullauto2 0`</span>
<span style="color:green; text-decoration:underline">`mineguided1 0`</span>
<span style="color:green; text-decoration:underline">`mineguided2 0`</span>
<span style="color:green; text-decoration:underline">`mineguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`mineguideddelay2 0`</span>
<span style="color:green; text-decoration:underline">`mineheadmin1 8.0`</span>
<span style="color:green; text-decoration:underline">`mineheadmin2 8.0`</span>
<span style="color:green; text-decoration:underline">`minehitpush1 0.0`</span>
<span style="color:green; text-decoration:underline">`minehitpush2 0.0`</span>
<span style="color:green; text-decoration:underline">`mineinteracts1 3`</span>
<span style="color:green; text-decoration:underline">`mineinteracts2 3`</span>
<span style="color:green; text-decoration:underline">`minekickpush1 5.0`</span>
<span style="color:green; text-decoration:underline">`minekickpush2 5.0`</span>
<span style="color:green; text-decoration:underline">`minelaser 0`</span>
<span style="color:green; text-decoration:underline">`minelegdamage1 0.2`</span>
<span style="color:green; text-decoration:underline">`minelegdamage2 0.2`</span>
<span style="color:green; text-decoration:underline">`minelimspeed1 0`</span>
<span style="color:green; text-decoration:underline">`minelimspeed2 0`</span>
<span style="color:green; text-decoration:underline">`minemax 2`</span>
<span style="color:green; text-decoration:underline">`mineminspeed1 0.0`</span>
<span style="color:green; text-decoration:underline">`mineminspeed2 0.0`</span>
<span style="color:green; text-decoration:underline">`minemodes -64`</span>
<span style="color:green; text-decoration:underline">`minemuts -24`</span>
<span style="color:green; text-decoration:underline">`minename "mine"`</span>
<span style="color:green; text-decoration:underline">`minepartcol1 0x00F068`</span>
<span style="color:green; text-decoration:underline">`minepartcol2 0x00F068`</span>
<span style="color:green; text-decoration:underline">`minepartlen1 4.0`</span>
<span style="color:green; text-decoration:underline">`minepartlen2 4.0`</span>
<span style="color:green; text-decoration:underline">`minepartsize1 2.0`</span>
<span style="color:green; text-decoration:underline">`minepartsize2 2.0`</span>
<span style="color:green; text-decoration:underline">`mineparttype1 9`</span>
<span style="color:green; text-decoration:underline">`mineparttype2 9`</span>
<span style="color:green; text-decoration:underline">`minepower1 0`</span>
<span style="color:green; text-decoration:underline">`minepower2 0`</span>
<span style="color:green; text-decoration:underline">`mineprojdelay1 75`</span>
<span style="color:green; text-decoration:underline">`mineprojdelay2 75`</span>
<span style="color:green; text-decoration:underline">`mineproxdelay1 3000`</span>
<span style="color:green; text-decoration:underline">`mineproxdelay2 1500000`</span>
<span style="color:green; text-decoration:underline">`mineproxdist1 32.0`</span>
<span style="color:green; text-decoration:underline">`mineproxdist2 1000000.0`</span>
<span style="color:green; text-decoration:underline">`mineproxtime1 100`</span>
<span style="color:green; text-decoration:underline">`mineproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`mineproxtype1 1`</span>
<span style="color:green; text-decoration:underline">`mineproxtype2 2`</span>
<span style="color:green; text-decoration:underline">`mineradial1 0`</span>
<span style="color:green; text-decoration:underline">`mineradial2 0`</span>
<span style="color:green; text-decoration:underline">`mineradius1 1.0`</span>
<span style="color:green; text-decoration:underline">`mineradius2 1.0`</span>
<span style="color:green; text-decoration:underline">`minerays1 1`</span>
<span style="color:green; text-decoration:underline">`minerays2 1`</span>
<span style="color:green; text-decoration:underline">`minereflectivity1 0.0`</span>
<span style="color:green; text-decoration:underline">`minereflectivity2 0.0`</span>
<span style="color:green; text-decoration:underline">`minerelativity1 1.0`</span>
<span style="color:green; text-decoration:underline">`minerelativity2 1.0`</span>
<span style="color:green; text-decoration:underline">`minereloaddelay 3000`</span>
<span style="color:green; text-decoration:underline">`minereloads 0`</span>
<span style="color:green; text-decoration:underline">`mineresidual1 4`</span>
<span style="color:green; text-decoration:underline">`mineresidual2 4`</span>
<span style="color:green; text-decoration:underline">`mineselfdamage1 0.5`</span>
<span style="color:green; text-decoration:underline">`mineselfdamage2 0.5`</span>
<span style="color:green; text-decoration:underline">`minespeed1 100`</span>
<span style="color:green; text-decoration:underline">`minespeed2 100`</span>
<span style="color:green; text-decoration:underline">`minespread1 1.0`</span>
<span style="color:green; text-decoration:underline">`minespread2 1.0`</span>
<span style="color:green; text-decoration:underline">`minespreadmax1 0.0`</span>
<span style="color:green; text-decoration:underline">`minespreadmax2 0.0`</span>
<span style="color:green; text-decoration:underline">`minespreadmin1 0.0`</span>
<span style="color:green; text-decoration:underline">`minespreadmin2 0.0`</span>
<span style="color:green; text-decoration:underline">`minespreadz1 0.0`</span>
<span style="color:green; text-decoration:underline">`minespreadz2 0.0`</span>
<span style="color:green; text-decoration:underline">`minestunfall1 8.0`</span>
<span style="color:green; text-decoration:underline">`minestunfall2 16.0`</span>
<span style="color:green; text-decoration:underline">`minestunscale1 8.0`</span>
<span style="color:green; text-decoration:underline">`minestunscale2 16.0`</span>
<span style="color:green; text-decoration:underline">`minestuntime1 500`</span>
<span style="color:green; text-decoration:underline">`minestuntime2 750`</span>
<span style="color:green; text-decoration:underline">`minesub1 1`</span>
<span style="color:green; text-decoration:underline">`minesub2 1`</span>
<span style="color:green; text-decoration:underline">`minetaper1 0`</span>
<span style="color:green; text-decoration:underline">`minetaper2 0`</span>
<span style="color:green; text-decoration:underline">`minetaperin1 0.0`</span>
<span style="color:green; text-decoration:underline">`minetaperin2 0.0`</span>
<span style="color:green; text-decoration:underline">`minetaperout1 0.0`</span>
<span style="color:green; text-decoration:underline">`minetaperout2 0.0`</span>
<span style="color:green; text-decoration:underline">`mineteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`mineteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`mineteampenalty1 0.0`</span>
<span style="color:green; text-decoration:underline">`mineteampenalty2 0.0`</span>
<span style="color:green; text-decoration:underline">`minetime1 60000`</span>
<span style="color:green; text-decoration:underline">`minetime2 30000`</span>
<span style="color:green; text-decoration:underline">`minetorsodamage1 0.4`</span>
<span style="color:green; text-decoration:underline">`minetorsodamage2 0.4`</span>
<span style="color:green; text-decoration:underline">`minetrace1 1.0`</span>
<span style="color:green; text-decoration:underline">`minetrace2 1.0`</span>
<span style="color:green; text-decoration:underline">`minevisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`minevisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`minevistime1 0`</span>
<span style="color:green; text-decoration:underline">`minevistime2 0`</span>
<span style="color:green; text-decoration:underline">`minewaterfric1 2.0`</span>
<span style="color:green; text-decoration:underline">`minewaterfric2 2.0`</span>
<span style="color:green; text-decoration:underline">`minewavepush1 2.0`</span>
<span style="color:green; text-decoration:underline">`minewavepush2 2.0`</span>
<span style="color:green; text-decoration:underline">`mineweight1 150.0`</span>
<span style="color:green; text-decoration:underline">`mineweight2 150.0`</span>
<span style="color:green; text-decoration:underline">`minewhipdamage1 0.6`</span>
<span style="color:green; text-decoration:underline">`minewhipdamage2 0.6`</span>
<span style="color:green; text-decoration:underline">`minezooms 0`</span>
`minresizescale 0.5`
<span style="color:green; text-decoration:underline">`modelock 4`</span>
<span style="color:green; text-decoration:underline">`modelockfilter 188`</span>
<span style="color:green; text-decoration:underline">`modelocktype 2`</span>
`movecrawl 0.6`
`moveinair 0.9`
`movejet 1.6`
<span style="color:green; text-decoration:underline">`movepacing 1.6`</span>
`movespeed 100.0`
`movespread 1.0`
<span style="color:red; text-decoration:line-through">`movesprint 1.6`</span>
`movestepdown 1.15`
`movestepup 0.95`
`movestrafe 1.0`
`multikillbonus 1`
`multikilldelay 5000`
`multikillpoints 1`
<span style="color:green; text-decoration:underline">`multimaps "canals deadsimple depot keystone2k warp fourplex"`</span>
<span style="color:green; text-decoration:underline">`mutelock 3`</span>
<span style="color:green; text-decoration:underline">`mutslockfilter 126975`</span>
<span style="color:green; text-decoration:underline">`numplayers 4`</span>
`overtimeallow 1`
`overtimelimit 5`
`pistoladd 10`
<span style="color:red; text-decoration:line-through">`pistoladelay1 150`</span>
<span style="color:red; text-decoration:line-through">`pistoladelay2 350`</span>
`pistolaidist1 256.0`
`pistolaidist2 256.0`
`pistolaiskew1 100`
`pistolaiskew2 100`
<span style="color:red; text-decoration:line-through">`pistolallowed 2`</span><span style="color:green; text-decoration:underline">`pistolattackdelay1 100`</span>
<span style="color:green; text-decoration:underline">`pistolattackdelay2 200`</span>
`pistolcarried 0`
`pistolcollide1 `<span style="color:red; text-decoration:line-through">`53`</span><span style="color:green; text-decoration:underline">`61`</span>
`pistolcollide2 `<span style="color:red; text-decoration:line-through">`53`</span><span style="color:green; text-decoration:underline">`61`</span>
`pistolcolour `<span style="color:red; text-decoration:line-through">`0x888888`</span><span style="color:green; text-decoration:underline">`0xC0C0C0`</span>
`pistolcooked1 0`
`pistolcooked2 0`
<span style="color:red; text-decoration:line-through">`pistolcritdash1 0`</span>
<span style="color:red; text-decoration:line-through">`pistolcritdash2 0`</span>
<span style="color:red; text-decoration:line-through">`pistolcritdist 128.0`</span>
<span style="color:red; text-decoration:line-through">`pistolcritmult 3.0`</span>
`pistoldamage2 `<span style="color:red; text-decoration:line-through">`3`</span><span style="color:green; text-decoration:underline">`40`</span>
`pistoldelta1 10.0`
`pistoldelta2 10.0`
<span style="color:red; text-decoration:line-through">`pistoledelay1 200`</span><span style="color:green; text-decoration:underline">`pistoldrill1 0`</span>
<span style="color:red; text-decoration:line-through">`pistoledelay2 200`</span><span style="color:green; text-decoration:underline">`pistoldrill2 0`</span>
`pistolelasticity1 0.5`
`pistolelasticity2 0.5`
<span style="color:green; text-decoration:underline">`pistolescapedelay1 200`</span>
<span style="color:green; text-decoration:underline">`pistolescapedelay2 200`</span>
`pistolexplcol1 -1`
`pistolexplcol2 -1`
`pistolexplode1 `<span style="color:red; text-decoration:line-through">`0`</span><span style="color:green; text-decoration:underline">`0.0`</span>
`pistolexplode2 `<span style="color:red; text-decoration:line-through">`0`</span><span style="color:green; text-decoration:underline">`0.0`</span>
`pistolextinguish1 2`
`pistolextinguish2 2`
`pistolflakcollide1 `<span style="color:red; text-decoration:line-through">`53`</span><span style="color:green; text-decoration:underline">`61`</span>
`pistolflakcollide2 `<span style="color:red; text-decoration:line-through">`53`</span><span style="color:green; text-decoration:underline">`61`</span>
<span style="color:red; text-decoration:line-through">`pistolflakdmg1 10`</span><span style="color:green; text-decoration:underline">`pistolflakdamage1 25`</span>
<span style="color:red; text-decoration:line-through">`pistolflakdmg2 12`</span><span style="color:green; text-decoration:underline">`pistolflakdamage2 40`</span>
<span style="color:red; text-decoration:line-through">`pistolflakffwd1`</span><span style="color:green; text-decoration:underline">`pistolflakdelta1 10.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakdelta2 10.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakdrill1 0`</span>
<span style="color:green; text-decoration:underline">`pistolflakdrill2 0`</span>
<span style="color:green; text-decoration:underline">`pistolflakelasticity1 0.5`</span>
<span style="color:green; text-decoration:underline">`pistolflakelasticity2 0.5`</span>
<span style="color:green; text-decoration:underline">`pistolflakexplcol1 -1`</span>
<span style="color:green; text-decoration:underline">`pistolflakexplcol2 -1`</span>
<span style="color:green; text-decoration:underline">`pistolflakexplode1`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`pistolflakffwd2`</span><span style="color:green; text-decoration:underline">`pistolflakexplode2`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`pistolflakminspeed1`</span><span style="color:green; text-decoration:underline">`pistolflakextinguish1 2`</span>
<span style="color:green; text-decoration:underline">`pistolflakextinguish2 2`</span>
<span style="color:green; text-decoration:underline">`pistolflakguided1 0`</span>
<span style="color:green; text-decoration:underline">`pistolflakguided2 0`</span>
<span style="color:green; text-decoration:underline">`pistolflakguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`pistolflakguideddelay2 0`</span>
<span style="color:green; text-decoration:underline">`pistolflakheadmin1 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakheadmin2`</span>` 0.0`
<span style="color:green; text-decoration:underline">`pistolflakhitpush1 35.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakhitpush2 75.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakinteracts1 1`</span>
<span style="color:green; text-decoration:underline">`pistolflakinteracts2 1`</span>
<span style="color:green; text-decoration:underline">`pistolflaklegdamage1 0.325`</span>
<span style="color:green; text-decoration:underline">`pistolflaklegdamage2 0.325`</span>
<span style="color:green; text-decoration:underline">`pistolflakminspeed1 50.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakpartcol1 0x666611`</span>
<span style="color:green; text-decoration:underline">`pistolflakpartcol2 0x666611`</span>
<span style="color:green; text-decoration:underline">`pistolflakpartlen1 10.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakpartlen2 15.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakpartsize1 2.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakpartsize2 2.5`</span>
<span style="color:green; text-decoration:underline">`pistolflakparttype1 1`</span>
<span style="color:green; text-decoration:underline">`pistolflakparttype2 1`</span>
<span style="color:green; text-decoration:underline">`pistolflakproxdelay1 0`</span>
<span style="color:green; text-decoration:underline">`pistolflakproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`pistolflakproxdist1 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakproxdist2 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`pistolflakproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`pistolflakproxtype1 0`</span>
<span style="color:green; text-decoration:underline">`pistolflakproxtype2 0`</span>
<span style="color:green; text-decoration:underline">`pistolflakradial1 0`</span>
<span style="color:green; text-decoration:underline">`pistolflakradial2 0`</span>
<span style="color:green; text-decoration:underline">`pistolflakradius1 1.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakradius2 1.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakreflectivity1 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakreflectivity2 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakresidual1 0`</span>
<span style="color:green; text-decoration:underline">`pistolflakresidual2 0`</span>
<span style="color:green; text-decoration:underline">`pistolflakselfdamage1 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakselfdamage2 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakstunfall1 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakstunfall2 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakstunscale1 0.25`</span>
<span style="color:green; text-decoration:underline">`pistolflakstunscale2 0.5`</span>
<span style="color:green; text-decoration:underline">`pistolflakstuntime1 25`</span>
<span style="color:green; text-decoration:underline">`pistolflakstuntime2 50`</span>
<span style="color:green; text-decoration:underline">`pistolflaktaper1 0`</span>
<span style="color:green; text-decoration:underline">`pistolflaktaper2 0`</span>
<span style="color:green; text-decoration:underline">`pistolflaktaperin1 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolflaktaperin2 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolflaktaperout1 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolflaktaperout2 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakteampenalty1 1.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakteampenalty2 1.0`</span>
<span style="color:green; text-decoration:underline">`pistolflaktorsodamage1 0.65`</span>
<span style="color:green; text-decoration:underline">`pistolflaktorsodamage2 0.65`</span>
<span style="color:green; text-decoration:underline">`pistolflakvisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakvisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakvistime1 0`</span>
<span style="color:green; text-decoration:underline">`pistolflakvistime2 0`</span>
<span style="color:green; text-decoration:underline">`pistolflakwaterfric1 2.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakwaterfric2 2.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakwavepush1 1.5`</span>
<span style="color:green; text-decoration:underline">`pistolflakwavepush2 1.5`</span>
<span style="color:green; text-decoration:underline">`pistolflakweight1 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakweight2 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolflakwhipdamage1 0.8`</span>
<span style="color:green; text-decoration:underline">`pistolflakwhipdamage2 0.8`</span>
<span style="color:green; text-decoration:underline">`pistolfragdelay1 0`</span>
<span style="color:green; text-decoration:underline">`pistolfragdelay2 0`</span>
<span style="color:green; text-decoration:underline">`pistolfragjump1 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolfragjump2`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`pistolflakoffset1 8.0`</span><span style="color:green; text-decoration:underline">`pistolfragoffset1 4.0`</span>
<span style="color:red; text-decoration:line-through">`pistolflakoffset2 8.0`</span><span style="color:green; text-decoration:underline">`pistolfragoffset2 4.0`</span>
<span style="color:red; text-decoration:line-through">`pistolflakrays1`</span><span style="color:green; text-decoration:underline">`pistolfragrays1`</span>` 5`
<span style="color:red; text-decoration:line-through">`pistolflakrays2`</span><span style="color:green; text-decoration:underline">`pistolfragrays2`</span>` 5`
<span style="color:red; text-decoration:line-through">`pistolflakrel1`</span><span style="color:green; text-decoration:underline">`pistolfragrel1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`pistolflakrel2`</span><span style="color:green; text-decoration:underline">`pistolfragrel2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`pistolflakscale1`</span><span style="color:green; text-decoration:underline">`pistolfragscale1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`pistolflakscale2`</span><span style="color:green; text-decoration:underline">`pistolfragscale2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`pistolflakskew1`</span><span style="color:green; text-decoration:underline">`pistolfragskew1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`pistolflakskew2`</span><span style="color:green; text-decoration:underline">`pistolfragskew2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`pistolflakspeed1`</span><span style="color:green; text-decoration:underline">`pistolfragspeed1`</span>` 0`
<span style="color:red; text-decoration:line-through">`pistolflakspeed2`</span><span style="color:green; text-decoration:underline">`pistolfragspeed2`</span>` 0`
<span style="color:red; text-decoration:line-through">`pistolflakspread1`</span><span style="color:green; text-decoration:underline">`pistolfragspread1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`pistolflakspread2`</span><span style="color:green; text-decoration:underline">`pistolfragspread2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`pistolflaktime1`</span><span style="color:green; text-decoration:underline">`pistolfragtime1`</span>` 500`
<span style="color:red; text-decoration:line-through">`pistolflaktime2`</span><span style="color:green; text-decoration:underline">`pistolfragtime2`</span>` 500`
<span style="color:red; text-decoration:line-through">`pistolflakweap1`</span><span style="color:green; text-decoration:underline">`pistolfragweap1`</span>` -1`
<span style="color:red; text-decoration:line-through">`pistolflakweap2`</span><span style="color:green; text-decoration:underline">`pistolfragweap2`</span>` -1`
`pistolfrequency 0.0`
`pistolfullauto1 0`
`pistolfullauto2 0`
<span style="color:red; text-decoration:line-through">`pistolgdelay1 0`</span>
<span style="color:red; text-decoration:line-through">`pistolgdelay2 0`</span>
`pistolguided1 0`
`pistolguided2 0`
<span style="color:green; text-decoration:underline">`pistolguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`pistolguideddelay2 0`</span>
`pistolheadmin1 0.0`
`pistolheadmin2 0.0`
`pistolhitpush1 35.0`
`pistolhitpush2 `<span style="color:red; text-decoration:line-through">`50.0`</span><span style="color:green; text-decoration:underline">`75.0`</span>
<span style="color:red; text-decoration:line-through">`pistoljamchance 10`</span><span style="color:green; text-decoration:underline">`pistolinteracts1 1`</span>
<span style="color:green; text-decoration:underline">`pistolinteracts2 1`</span>
`pistolkickpush1 `<span style="color:red; text-decoration:line-through">`6.0`</span><span style="color:green; text-decoration:underline">`4.0`</span>
`pistolkickpush2 `<span style="color:red; text-decoration:line-through">`4.0`</span><span style="color:green; text-decoration:underline">`8.0`</span>
`pistollaser 0`
<span style="color:red; text-decoration:line-through">`pistollegsdmg1`</span><span style="color:green; text-decoration:underline">`pistollegdamage1`</span>` 0.325`
<span style="color:red; text-decoration:line-through">`pistollegsdmg2`</span><span style="color:green; text-decoration:underline">`pistollegdamage2`</span>` 0.325`
`pistollimspeed1 0`
`pistollimspeed2 0`
`pistolmax 10`
<span style="color:red; text-decoration:line-through">`pistolmaxspread1 0`</span>
<span style="color:red; text-decoration:line-through">`pistolmaxspread2 0`</span>
`pistolminspeed1 0.0`
`pistolminspeed2 0.0`
<span style="color:red; text-decoration:line-through">`pistolminspread1 0`</span><span style="color:green; text-decoration:underline">`pistolmodes -64`</span>
<span style="color:red; text-decoration:line-through">`pistolminspread2 0`</span><span style="color:green; text-decoration:underline">`pistolmuts -56`</span>
`pistolname "pistol"`
`pistolpartcol1 0x666611`
`pistolpartcol2 0x666611`
`pistolpartlen1 10.0`
`pistolpartlen2 `<span style="color:red; text-decoration:line-through">`10.0`</span><span style="color:green; text-decoration:underline">`15.0`</span>
`pistolpartsize1 2.0`
`pistolpartsize2 `<span style="color:red; text-decoration:line-through">`0.5`</span><span style="color:green; text-decoration:underline">`2.5`</span>
`pistolparttype1 1`
`pistolparttype2 1`
<span style="color:red; text-decoration:line-through">`pistolpdelay1 0`</span>
<span style="color:red; text-decoration:line-through">`pistolpdelay2 0`</span>
`pistolpower1 0`
`pistolpower2 0`
<span style="color:red; text-decoration:line-through">`pistolpusharea 1.0`</span><span style="color:green; text-decoration:underline">`pistolprojdelay1 0`</span>
<span style="color:green; text-decoration:underline">`pistolprojdelay2 0`</span>
<span style="color:green; text-decoration:underline">`pistolproxdelay1 0`</span>
<span style="color:green; text-decoration:underline">`pistolproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`pistolproxdist1 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolproxdist2 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`pistolproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`pistolproxtype1 0`</span>
<span style="color:green; text-decoration:underline">`pistolproxtype2 0`</span>
`pistolradial1 0`
`pistolradial2 0`
`pistolradius1 1.0`
`pistolradius2 1.0`
`pistolrays1 1`
`pistolrays2 `<span style="color:red; text-decoration:line-through">`10`</span>
<span style="color:red; text-decoration:line-through">`pistolrdelay 1000`</span><span style="color:green; text-decoration:underline">`1`</span>
`pistolreflectivity1 0.0`
`pistolreflectivity2 0.0`
`pistolrelativity1 0.05`
`pistolrelativity2 0.05`
<span style="color:green; text-decoration:underline">`pistolreloaddelay 1000`</span>
`pistolreloads -1`
`pistolresidual1 0`
`pistolresidual2 0`
<span style="color:red; text-decoration:line-through">`pistolselfdmg1`</span><span style="color:green; text-decoration:underline">`pistolselfdamage1`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`pistolselfdmg2 0.0`</span>
<span style="color:red; text-decoration:line-through">`pistolslow1 0.0`</span>
<span style="color:red; text-decoration:line-through">`pistolslow2`</span><span style="color:green; text-decoration:underline">`pistolselfdamage2`</span>` 0.0`
`pistolspeed1 `<span style="color:red; text-decoration:line-through">`3000`</span><span style="color:green; text-decoration:underline">`1750`</span>
`pistolspeed2 1000`
`pistolspread1 `<span style="color:red; text-decoration:line-through">`1`</span><span style="color:green; text-decoration:underline">`1.0`</span>
`pistolspread2 `<span style="color:red; text-decoration:line-through">`10`</span><span style="color:green; text-decoration:underline">`2.0`</span>
<span style="color:green; text-decoration:underline">`pistolspreadmax1 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolspreadmax2 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolspreadmin1 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolspreadmin2 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolspreadz1 2.0`</span>
<span style="color:green; text-decoration:underline">`pistolspreadz2 4.0`</span>
<span style="color:green; text-decoration:underline">`pistolstunfall1 0.0`</span>
<span style="color:green; text-decoration:underline">`pistolstunfall2 0.0`</span>
`pistolstunscale1 0.25`
`pistolstunscale2 `<span style="color:red; text-decoration:line-through">`0.25`</span><span style="color:green; text-decoration:underline">`0.5`</span>
`pistolstuntime1 25`
`pistolstuntime2 `<span style="color:red; text-decoration:line-through">`25`</span><span style="color:green; text-decoration:underline">`50`</span>
`pistolsub1 1`
`pistolsub2 2`
<span style="color:green; text-decoration:underline">`pistoltaper1 0`</span>
<span style="color:green; text-decoration:underline">`pistoltaper2 0`</span>
`pistoltaperin1 0.0`
`pistoltaperin2 0.0`
`pistoltaperout1 0.0`
`pistoltaperout2 0.0`
<span style="color:green; text-decoration:underline">`pistolteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`pistolteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`pistolteampenalty1 1.0`</span>
<span style="color:green; text-decoration:underline">`pistolteampenalty2 1.0`</span>
`pistoltime1 2000`
`pistoltime2 `<span style="color:red; text-decoration:line-through">`400`</span><span style="color:green; text-decoration:underline">`1000`</span>
<span style="color:red; text-decoration:line-through">`pistoltorsodmg1`</span><span style="color:green; text-decoration:underline">`pistoltorsodamage1`</span>` 0.65`
<span style="color:red; text-decoration:line-through">`pistoltorsodmg2`</span><span style="color:green; text-decoration:underline">`pistoltorsodamage2`</span>` 0.65`
`pistoltrace1 1.0`
`pistoltrace2 1.0`
<span style="color:green; text-decoration:underline">`pistolvisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`pistolvisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`pistolvistime1 0`</span>
<span style="color:green; text-decoration:underline">`pistolvistime2 0`</span>
`pistolwaterfric1 2.0`
`pistolwaterfric2 2.0`
<span style="color:green; text-decoration:underline">`pistolwavepush1 1.5`</span>
<span style="color:green; text-decoration:underline">`pistolwavepush2 1.5`</span>
`pistolweight1 0.0`
`pistolweight2 0.0`
<span style="color:red; text-decoration:line-through">`pistolwhipdmg1`</span><span style="color:green; text-decoration:underline">`pistolwhipdamage1`</span>` 0.8`
<span style="color:red; text-decoration:line-through">`pistolwhipdmg2`</span><span style="color:green; text-decoration:underline">`pistolwhipdamage2`</span>` 0.8 `<span style="color:red; text-decoration:line-through">`pistolzdiv1 2`</span>
<span style="color:red; text-decoration:line-through">`pistolzdiv2 1`</span>
`pistolzooms 0`
`plasmaadd `<span style="color:red; text-decoration:line-through">`20`</span>
<span style="color:red; text-decoration:line-through">`plasmaadelay1 300`</span>
<span style="color:red; text-decoration:line-through">`plasmaadelay2 1000`</span><span style="color:green; text-decoration:underline">`16`</span>
`plasmaaidist1 128.0`
`plasmaaidist2 64.0`
`plasmaaiskew1 50`
`plasmaaiskew2 10`
<span style="color:red; text-decoration:line-through">`plasmaallowed 2`</span><span style="color:green; text-decoration:underline">`plasmaattackdelay1 350`</span>
<span style="color:green; text-decoration:underline">`plasmaattackdelay2 1500`</span>
`plasmacarried 1`
`plasmacollide1 `<span style="color:red; text-decoration:line-through">`85`</span><span style="color:green; text-decoration:underline">`60`</span>
`plasmacollide2 `<span style="color:red; text-decoration:line-through">`337`</span><span style="color:green; text-decoration:underline">`4140`</span>
`plasmacolour `<span style="color:red; text-decoration:line-through">`0x44DDCC`</span><span style="color:green; text-decoration:underline">`0x40F0C8`</span>
`plasmacooked1 0`
`plasmacooked2 33`
<span style="color:red; text-decoration:line-through">`plasmacritdash1 0`</span>
<span style="color:red; text-decoration:line-through">`plasmacritdash2 0`</span>
<span style="color:red; text-decoration:line-through">`plasmacritdist 0.0`</span>
<span style="color:red; text-decoration:line-through">`plasmacritmult 2.0`</span>
`plasmadamage2 10`
`plasmadelta1 10.0`
`plasmadelta2 10.0`
<span style="color:red; text-decoration:line-through">`plasmaedelay1 200`</span><span style="color:green; text-decoration:underline">`plasmadrill1 0`</span>
<span style="color:red; text-decoration:line-through">`plasmaedelay2 200`</span><span style="color:green; text-decoration:underline">`plasmadrill2 0`</span>
`plasmaelasticity1 0.5`
`plasmaelasticity2 0.5`
<span style="color:green; text-decoration:underline">`plasmaescapedelay1 200`</span>
<span style="color:green; text-decoration:underline">`plasmaescapedelay2 200`</span>
`plasmaexplcol2 `<span style="color:red; text-decoration:line-through">`0x44DDCC`</span><span style="color:green; text-decoration:underline">`0x40F0C8`</span>
`plasmaexplode1 `<span style="color:red; text-decoration:line-through">`8`</span><span style="color:green; text-decoration:underline">`10.0`</span>
`plasmaexplode2 `<span style="color:red; text-decoration:line-through">`48`</span><span style="color:green; text-decoration:underline">`48.0`</span>
`plasmaextinguish1 1`
`plasmaextinguish2 0`
`plasmaflakcollide1 `<span style="color:red; text-decoration:line-through">`85`</span><span style="color:green; text-decoration:underline">`60`</span>
`plasmaflakcollide2 `<span style="color:red; text-decoration:line-through">`337`</span><span style="color:green; text-decoration:underline">`12332`</span>
<span style="color:red; text-decoration:line-through">`plasmaflakdmg1`</span><span style="color:green; text-decoration:underline">`plasmaflakdamage1 22`</span>
<span style="color:green; text-decoration:underline">`plasmaflakdamage2`</span>` 10`
<span style="color:red; text-decoration:line-through">`plasmaflakdmg2 5`</span><span style="color:green; text-decoration:underline">`plasmaflakdelta1 10.0`</span>
<span style="color:red; text-decoration:line-through">`plasmaflakffwd1 0.0`</span><span style="color:green; text-decoration:underline">`plasmaflakdelta2 10.0`</span>
<span style="color:red; text-decoration:line-through">`plasmaflakffwd2 0.0`</span><span style="color:green; text-decoration:underline">`plasmaflakdrill1 0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakdrill2 0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakelasticity1 0.5`</span>
<span style="color:green; text-decoration:underline">`plasmaflakelasticity2 0.5`</span>
<span style="color:green; text-decoration:underline">`plasmaflakexplcol1 0x40F0C8`</span>
<span style="color:green; text-decoration:underline">`plasmaflakexplcol2 0x40F0C8`</span>
<span style="color:green; text-decoration:underline">`plasmaflakexplode1 10.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakexplode2 48.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakextinguish1 1`</span>
<span style="color:green; text-decoration:underline">`plasmaflakextinguish2 0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakguided1 0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakguided2 0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakguideddelay2 0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakheadmin1 8.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakheadmin2 4.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakhitpush1 20.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakhitpush2 -100.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakinteracts1 1`</span>
<span style="color:green; text-decoration:underline">`plasmaflakinteracts2 1`</span>
<span style="color:green; text-decoration:underline">`plasmaflaklegdamage1 0.2`</span>
<span style="color:green; text-decoration:underline">`plasmaflaklegdamage2 0.2`</span>
`plasmaflakminspeed1 `<span style="color:red; text-decoration:line-through">`0.0`</span><span style="color:green; text-decoration:underline">`50.0`</span>
`plasmaflakminspeed2 `<span style="color:green; text-decoration:underline">`50.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakpartcol1 0x40F0C8`</span>
<span style="color:green; text-decoration:underline">`plasmaflakpartcol2 0x40F0C8`</span>
<span style="color:green; text-decoration:underline">`plasmaflakpartlen1`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`plasmaflakoffset1 8.0`</span><span style="color:green; text-decoration:underline">`plasmaflakpartlen2 0.0`</span>
<span style="color:red; text-decoration:line-through">`plasmaflakoffset2`</span><span style="color:green; text-decoration:underline">`plasmaflakpartsize1`</span>` 8.0`
<span style="color:red; text-decoration:line-through">`plasmaflakrays1`</span><span style="color:green; text-decoration:underline">`plasmaflakpartsize2 24.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakparttype1 6`</span>
<span style="color:green; text-decoration:underline">`plasmaflakparttype2 6`</span>
<span style="color:green; text-decoration:underline">`plasmaflakproxdelay1 0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakproxdist1 0.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakproxdist2 0.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakproxtype1 0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakproxtype2 0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakradial1 10`</span>
<span style="color:green; text-decoration:underline">`plasmaflakradial2 80`</span>
<span style="color:green; text-decoration:underline">`plasmaflakradius1 2.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakradius2 2.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakreflectivity1 0.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakreflectivity2 0.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakresidual1 0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakresidual2 0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakselfdamage1 0.5`</span>
<span style="color:green; text-decoration:underline">`plasmaflakselfdamage2 0.5`</span>
<span style="color:green; text-decoration:underline">`plasmaflakstunfall1 0.5`</span>
<span style="color:green; text-decoration:underline">`plasmaflakstunfall2 1.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakstunscale1 0.5`</span>
<span style="color:green; text-decoration:underline">`plasmaflakstunscale2 1.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakstuntime1 100`</span>
<span style="color:green; text-decoration:underline">`plasmaflakstuntime2 200`</span>
<span style="color:green; text-decoration:underline">`plasmaflaktaper1 1`</span>
<span style="color:green; text-decoration:underline">`plasmaflaktaper2 2`</span>
<span style="color:green; text-decoration:underline">`plasmaflaktaperin1 0.00625`</span>
<span style="color:green; text-decoration:underline">`plasmaflaktaperin2 0.5`</span>
<span style="color:green; text-decoration:underline">`plasmaflaktaperout1 0.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflaktaperout2 0.5`</span>
<span style="color:green; text-decoration:underline">`plasmaflakteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakteampenalty1 1.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakteampenalty2 0.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflaktorsodamage1 0.4`</span>
<span style="color:green; text-decoration:underline">`plasmaflaktorsodamage2 0.4`</span>
<span style="color:green; text-decoration:underline">`plasmaflakvisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakvisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakvistime1 0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakvistime2 0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakwaterfric1 1.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakwaterfric2 1.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakwavepush1 1.5`</span>
<span style="color:green; text-decoration:underline">`plasmaflakwavepush2 2.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakweight1 0.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakweight2 0.0`</span>
<span style="color:green; text-decoration:underline">`plasmaflakwhipdamage1 0.6`</span>
<span style="color:green; text-decoration:underline">`plasmaflakwhipdamage2 0.6`</span>
<span style="color:green; text-decoration:underline">`plasmafragdelay1 0`</span>
<span style="color:green; text-decoration:underline">`plasmafragdelay2 0`</span>
<span style="color:green; text-decoration:underline">`plasmafragjump1 0.0`</span>
<span style="color:green; text-decoration:underline">`plasmafragjump2 0.0`</span>
<span style="color:green; text-decoration:underline">`plasmafragoffset1 4.0`</span>
<span style="color:green; text-decoration:underline">`plasmafragoffset2 4.0`</span>
<span style="color:green; text-decoration:underline">`plasmafragrays1`</span>` 5`
<span style="color:red; text-decoration:line-through">`plasmaflakrays2`</span><span style="color:green; text-decoration:underline">`plasmafragrays2`</span>` 5`
<span style="color:red; text-decoration:line-through">`plasmaflakrel1`</span><span style="color:green; text-decoration:underline">`plasmafragrel1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`plasmaflakrel2`</span><span style="color:green; text-decoration:underline">`plasmafragrel2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`plasmaflakscale1`</span><span style="color:green; text-decoration:underline">`plasmafragscale1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`plasmaflakscale2`</span><span style="color:green; text-decoration:underline">`plasmafragscale2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`plasmaflakskew1`</span><span style="color:green; text-decoration:underline">`plasmafragskew1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`plasmaflakskew2`</span><span style="color:green; text-decoration:underline">`plasmafragskew2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`plasmaflakspeed1`</span><span style="color:green; text-decoration:underline">`plasmafragspeed1`</span>` 0`
<span style="color:red; text-decoration:line-through">`plasmaflakspeed2`</span><span style="color:green; text-decoration:underline">`plasmafragspeed2`</span>` 0`
<span style="color:red; text-decoration:line-through">`plasmaflakspread1`</span><span style="color:green; text-decoration:underline">`plasmafragspread1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`plasmaflakspread2`</span><span style="color:green; text-decoration:underline">`plasmafragspread2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`plasmaflaktime1`</span><span style="color:green; text-decoration:underline">`plasmafragtime1`</span>` 500`
<span style="color:red; text-decoration:line-through">`plasmaflaktime2`</span><span style="color:green; text-decoration:underline">`plasmafragtime2`</span>` 500`
<span style="color:red; text-decoration:line-through">`plasmaflakweap1`</span><span style="color:green; text-decoration:underline">`plasmafragweap1`</span>` -1`
<span style="color:red; text-decoration:line-through">`plasmaflakweap2`</span><span style="color:green; text-decoration:underline">`plasmafragweap2`</span>` -1`
`plasmafrequency 1.0`
`plasmafullauto1 1`
`plasmafullauto2 0`
<span style="color:red; text-decoration:line-through">`plasmagdelay1 0`</span>
<span style="color:red; text-decoration:line-through">`plasmagdelay2 0`</span>
`plasmaguided1 0`
`plasmaguided2 0`
<span style="color:green; text-decoration:underline">`plasmaguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`plasmaguideddelay2 0`</span>
`plasmaheadmin1 8.0`
`plasmaheadmin2 4.0`
`plasmahitpush1 20.0`
`plasmahitpush2 -100.0`
<span style="color:red; text-decoration:line-through">`plasmajamchance 35`</span><span style="color:green; text-decoration:underline">`plasmainteracts1 1`</span>
<span style="color:green; text-decoration:underline">`plasmainteracts2 1`</span>
`plasmakickpush1 25.0`
`plasmakickpush2 150.0`
`plasmalaser 0`
<span style="color:red; text-decoration:line-through">`plasmalegsdmg1`</span><span style="color:green; text-decoration:underline">`plasmalegdamage1`</span>` 0.2`
<span style="color:red; text-decoration:line-through">`plasmalegsdmg2`</span><span style="color:green; text-decoration:underline">`plasmalegdamage2`</span>` 0.2`
`plasmalimspeed1 0`
`plasmalimspeed2 35`
`plasmamax `<span style="color:red; text-decoration:line-through">`20`</span>
<span style="color:red; text-decoration:line-through">`plasmamaxspread1 0`</span>
<span style="color:red; text-decoration:line-through">`plasmamaxspread2 0`</span><span style="color:green; text-decoration:underline">`16`</span>
`plasmaminspeed1 0.0`
`plasmaminspeed2 0.0`
<span style="color:red; text-decoration:line-through">`plasmaminspread1 0`</span><span style="color:green; text-decoration:underline">`plasmamodes -64`</span>
<span style="color:red; text-decoration:line-through">`plasmaminspread2 0`</span><span style="color:green; text-decoration:underline">`plasmamuts -56`</span>
`plasmaname "plasma"`
`plasmapartcol1 `<span style="color:red; text-decoration:line-through">`0x44DDCC`</span><span style="color:green; text-decoration:underline">`0x40F0C8`</span>
`plasmapartcol2 `<span style="color:red; text-decoration:line-through">`0x44DDCC`</span><span style="color:green; text-decoration:underline">`0x40F0C8`</span>
`plasmapartlen1 0.0`
`plasmapartlen2 0.0`
`plasmapartsize1 `<span style="color:red; text-decoration:line-through">`6.0`</span><span style="color:green; text-decoration:underline">`8.0`</span>
`plasmapartsize2 24.0`
`plasmaparttype1 6`
`plasmaparttype2 6`
<span style="color:red; text-decoration:line-through">`plasmapdelay1 0`</span>
<span style="color:red; text-decoration:line-through">`plasmapdelay2 75`</span>
`plasmapower1 0`
`plasmapower2 2000`
<span style="color:red; text-decoration:line-through">`plasmapusharea 1.5`</span><span style="color:green; text-decoration:underline">`plasmaprojdelay1 0`</span>
<span style="color:green; text-decoration:underline">`plasmaprojdelay2 75`</span>
<span style="color:green; text-decoration:underline">`plasmaproxdelay1 0`</span>
<span style="color:green; text-decoration:underline">`plasmaproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`plasmaproxdist1 0.0`</span>
<span style="color:green; text-decoration:underline">`plasmaproxdist2 0.0`</span>
<span style="color:green; text-decoration:underline">`plasmaproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`plasmaproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`plasmaproxtype1 0`</span>
<span style="color:green; text-decoration:underline">`plasmaproxtype2 0`</span>
`plasmaradial1 `<span style="color:red; text-decoration:line-through">`8`</span><span style="color:green; text-decoration:underline">`10`</span>
`plasmaradial2 `<span style="color:red; text-decoration:line-through">`100`</span><span style="color:green; text-decoration:underline">`80`</span>
`plasmaradius1 2.0`
`plasmaradius2 2.0`
`plasmarays1 1`
`plasmarays2 1`
<span style="color:red; text-decoration:line-through">`plasmardelay 2000`</span>
`plasmareflectivity1 0.0`
`plasmareflectivity2 0.0`
`plasmarelativity1 0.1`
`plasmarelativity2 0.1`
<span style="color:green; text-decoration:underline">`plasmareloaddelay 2000`</span>
`plasmareloads -1`
`plasmaresidual1 0`
`plasmaresidual2 0`
<span style="color:red; text-decoration:line-through">`plasmaselfdmg1`</span><span style="color:green; text-decoration:underline">`plasmaselfdamage1`</span>` 0.5`
<span style="color:red; text-decoration:line-through">`plasmaselfdmg2`</span><span style="color:green; text-decoration:underline">`plasmaselfdamage2`</span>` 0.5`
<span style="color:red; text-decoration:line-through">`plasmaslow2 0.2`</span>
`plasmaspeed2 85`
`plasmaspread1 `<span style="color:red; text-decoration:line-through">`2`</span><span style="color:green; text-decoration:underline">`2.0`</span>
`plasmaspread2 `<span style="color:red; text-decoration:line-through">`1`</span><span style="color:green; text-decoration:underline">`1.0`</span>
<span style="color:green; text-decoration:underline">`plasmaspreadmax1 0.0`</span>
<span style="color:green; text-decoration:underline">`plasmaspreadmax2 0.0`</span>
<span style="color:green; text-decoration:underline">`plasmaspreadmin1 0.0`</span>
<span style="color:green; text-decoration:underline">`plasmaspreadmin2 0.0`</span>
<span style="color:green; text-decoration:underline">`plasmaspreadz1 2.0`</span>
<span style="color:green; text-decoration:underline">`plasmaspreadz2 1.0`</span>
<span style="color:green; text-decoration:underline">`plasmastunfall1 0.5`</span>
<span style="color:green; text-decoration:underline">`plasmastunfall2 1.0`</span>
`plasmastunscale1 0.5`
`plasmastunscale2 1.0`
`plasmastuntime1 `<span style="color:red; text-decoration:line-through">`50`</span><span style="color:green; text-decoration:underline">`100`</span>
`plasmastuntime2 `<span style="color:red; text-decoration:line-through">`50`</span><span style="color:green; text-decoration:underline">`200`</span>
`plasmasub1 1`
`plasmasub2 `<span style="color:red; text-decoration:line-through">`20`</span><span style="color:green; text-decoration:underline">`16`</span>
<span style="color:green; text-decoration:underline">`plasmataper1 1`</span>
<span style="color:green; text-decoration:underline">`plasmataper2 2`</span>
`plasmataperin1 `<span style="color:red; text-decoration:line-through">`0.05`</span><span style="color:green; text-decoration:underline">`0.00625`</span>
`plasmataperin2 0.5`
`plasmataperout1 0.0`
`plasmataperout2 0.5`
<span style="color:green; text-decoration:underline">`plasmateamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`plasmateamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`plasmateampenalty1 1.0`</span>
<span style="color:green; text-decoration:underline">`plasmateampenalty2 0.0`</span>
`plasmatime2 5000`
<span style="color:red; text-decoration:line-through">`plasmatorsodmg1`</span><span style="color:green; text-decoration:underline">`plasmatorsodamage1`</span>` 0.4`
<span style="color:red; text-decoration:line-through">`plasmatorsodmg2`</span><span style="color:green; text-decoration:underline">`plasmatorsodamage2`</span>` 0.4`
`plasmatrace1 1.0`
`plasmatrace2 1.0`
<span style="color:green; text-decoration:underline">`plasmavisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`plasmavisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`plasmavistime1 0`</span>
<span style="color:green; text-decoration:underline">`plasmavistime2 0`</span>
`plasmawaterfric1 1.0`
`plasmawaterfric2 1.0`
<span style="color:green; text-decoration:underline">`plasmawavepush1 1.5`</span>
<span style="color:green; text-decoration:underline">`plasmawavepush2 2.0`</span>
`plasmaweight1 0.0`
`plasmaweight2 0.0`
<span style="color:red; text-decoration:line-through">`plasmawhipdmg1`</span><span style="color:green; text-decoration:underline">`plasmawhipdamage1`</span>` 0.6`
<span style="color:red; text-decoration:line-through">`plasmawhipdmg2`</span><span style="color:green; text-decoration:underline">`plasmawhipdamage2`</span>` 0.6 `<span style="color:red; text-decoration:line-through">`plasmazdiv1 2`</span>
<span style="color:red; text-decoration:line-through">`plasmazdiv2 1`</span>
`plasmazooms 0`
`pointlimit 0`
<span style="color:green; text-decoration:underline">`previousmaps ""`</span>
<span style="color:green; text-decoration:underline">`pushlimited 0.75`</span>
<span style="color:green; text-decoration:underline">`pushscale 1.0`</span>
`quakefade 250`
<span style="color:green; text-decoration:underline">`quakelimit 200`</span>
<span style="color:green; text-decoration:underline">`radiallimited 0.75`</span>
<span style="color:green; text-decoration:underline">`radialscale 1.0`</span>
`regendecay 3`
`regendelay 3000`
`regenhealth 5`
`regentime 1000`
<span style="color:green; text-decoration:underline">`resetallowsonend 1`</span>
<span style="color:green; text-decoration:underline">`resetbansonend 1`</span>
<span style="color:green; text-decoration:underline">`resetlimitsonend 1`</span>
<span style="color:green; text-decoration:underline">`resetmmonend 2`</span>
<span style="color:green; text-decoration:underline">`resetmutesonend 1`</span>
<span style="color:green; text-decoration:underline">`resetvarsonend 1`</span>
`revengepoints 1`
`rifleadd `<span style="color:red; text-decoration:line-through">`5`</span>
<span style="color:red; text-decoration:line-through">`rifleadelay1 750`</span>
<span style="color:red; text-decoration:line-through">`rifleadelay2 1000`</span><span style="color:green; text-decoration:underline">`6`</span>
`rifleaidist1 768.0`
`rifleaidist2 2048.0`
`rifleaiskew1 40`
`rifleaiskew2 40`
<span style="color:red; text-decoration:line-through">`rifleallowed 2`</span><span style="color:green; text-decoration:underline">`rifleattackdelay1 750`</span>
<span style="color:green; text-decoration:underline">`rifleattackdelay2 1250`</span>
`riflecarried 1`
`riflecollide1 `<span style="color:red; text-decoration:line-through">`117`</span><span style="color:green; text-decoration:underline">`573`</span>
`riflecollide2 `<span style="color:red; text-decoration:line-through">`181`</span><span style="color:green; text-decoration:underline">`1597`</span>
`riflecolour `<span style="color:red; text-decoration:line-through">`0x8822DD`</span><span style="color:green; text-decoration:underline">`0xA020F0`</span>
`riflecooked1 0`
`riflecooked2 0`
<span style="color:red; text-decoration:line-through">`riflecritdash1 0`</span>
<span style="color:red; text-decoration:line-through">`riflecritdash2 0`</span>
<span style="color:red; text-decoration:line-through">`riflecritdist 1024.0`</span>
<span style="color:red; text-decoration:line-through">`riflecritmult 2.0`</span>
`rifledamage2 150`
`rifledelta1 10.0`
`rifledelta2 10.0`
<span style="color:red; text-decoration:line-through">`rifleedelay1 200`</span><span style="color:green; text-decoration:underline">`rifledrill1 2`</span>
<span style="color:red; text-decoration:line-through">`rifleedelay2 200`</span><span style="color:green; text-decoration:underline">`rifledrill2 8`</span>
`rifleelasticity1 0.5`
`rifleelasticity2 0.5`
<span style="color:green; text-decoration:underline">`rifleescapedelay1 200`</span>
<span style="color:green; text-decoration:underline">`rifleescapedelay2 200`</span>
`rifleexplcol2 `<span style="color:red; text-decoration:line-through">`0x8822DD`</span><span style="color:green; text-decoration:underline">`0xA020F0`</span>
`rifleexplode1 `<span style="color:red; text-decoration:line-through">`32`</span><span style="color:green; text-decoration:underline">`8.0`</span>
`rifleexplode2 `<span style="color:red; text-decoration:line-through">`0`</span><span style="color:green; text-decoration:underline">`0.0`</span>
`rifleextinguish1 2`
`rifleextinguish2 2`
`rifleflakcollide1 `<span style="color:red; text-decoration:line-through">`117`</span><span style="color:green; text-decoration:underline">`61`</span>
`rifleflakcollide2 `<span style="color:red; text-decoration:line-through">`181`</span><span style="color:green; text-decoration:underline">`1085`</span>
<span style="color:red; text-decoration:line-through">`rifleflakdmg1 18`</span><span style="color:green; text-decoration:underline">`rifleflakdamage1 10`</span>
<span style="color:red; text-decoration:line-through">`rifleflakdmg2 50`</span><span style="color:green; text-decoration:underline">`rifleflakdamage2 10`</span>
<span style="color:red; text-decoration:line-through">`rifleflakffwd1`</span><span style="color:green; text-decoration:underline">`rifleflakdelta1 10.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakdelta2 10.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakdrill1 2`</span>
<span style="color:green; text-decoration:underline">`rifleflakdrill2 8`</span>
<span style="color:green; text-decoration:underline">`rifleflakelasticity1 0.5`</span>
<span style="color:green; text-decoration:underline">`rifleflakelasticity2 0.5`</span>
<span style="color:green; text-decoration:underline">`rifleflakexplcol1 0x00F068`</span>
<span style="color:green; text-decoration:underline">`rifleflakexplcol2 0x00F068`</span>
<span style="color:green; text-decoration:underline">`rifleflakexplode1 4.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakexplode2 8.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakextinguish1 2`</span>
<span style="color:green; text-decoration:underline">`rifleflakextinguish2 2`</span>
<span style="color:green; text-decoration:underline">`rifleflakguided1 0`</span>
<span style="color:green; text-decoration:underline">`rifleflakguided2 0`</span>
<span style="color:green; text-decoration:underline">`rifleflakguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`rifleflakguideddelay2 0`</span>
<span style="color:green; text-decoration:underline">`rifleflakheadmin1 4.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakheadmin2 4.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakhitpush1`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`rifleflakffwd2`</span><span style="color:green; text-decoration:underline">`rifleflakhitpush2`</span>` 0.0`
<span style="color:green; text-decoration:underline">`rifleflakinteracts1 1`</span>
<span style="color:green; text-decoration:underline">`rifleflakinteracts2 1`</span>
<span style="color:green; text-decoration:underline">`rifleflaklegdamage1 0.2`</span>
<span style="color:green; text-decoration:underline">`rifleflaklegdamage2 0.2`</span>
`rifleflakminspeed2 `<span style="color:green; text-decoration:underline">`50.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakpartcol1 0x00F068`</span>
<span style="color:green; text-decoration:underline">`rifleflakpartcol2 0x00F068`</span>
<span style="color:green; text-decoration:underline">`rifleflakpartlen1 256.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakpartlen2 1024.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakpartsize1 0.75`</span>
<span style="color:green; text-decoration:underline">`rifleflakpartsize2 4.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakparttype1 7`</span>
<span style="color:green; text-decoration:underline">`rifleflakparttype2 7`</span>
<span style="color:green; text-decoration:underline">`rifleflakproxdelay1 0`</span>
<span style="color:green; text-decoration:underline">`rifleflakproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`rifleflakproxdist1 0.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakproxdist2 0.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`rifleflakproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`rifleflakproxtype1 0`</span>
<span style="color:green; text-decoration:underline">`rifleflakproxtype2 0`</span>
<span style="color:green; text-decoration:underline">`rifleflakradial1 0`</span>
<span style="color:green; text-decoration:underline">`rifleflakradial2 0`</span>
<span style="color:green; text-decoration:underline">`rifleflakradius1 1.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakradius2 1.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakreflectivity1 0.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakreflectivity2`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`rifleflakoffset1`</span><span style="color:green; text-decoration:underline">`rifleflakresidual1 4`</span>
<span style="color:green; text-decoration:underline">`rifleflakresidual2 4`</span>
<span style="color:green; text-decoration:underline">`rifleflakselfdamage1 0.5`</span>
<span style="color:green; text-decoration:underline">`rifleflakselfdamage2 0.5`</span>
<span style="color:green; text-decoration:underline">`rifleflakstunfall1`</span>` 8.0`
<span style="color:red; text-decoration:line-through">`rifleflakoffset2`</span><span style="color:green; text-decoration:underline">`rifleflakstunfall2 16.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakstunscale1`</span>` 8.0`
<span style="color:red; text-decoration:line-through">`rifleflakrays1`</span><span style="color:green; text-decoration:underline">`rifleflakstunscale2 16.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakstuntime1 500`</span>
<span style="color:green; text-decoration:underline">`rifleflakstuntime2 750`</span>
<span style="color:green; text-decoration:underline">`rifleflaktaper1 0`</span>
<span style="color:green; text-decoration:underline">`rifleflaktaper2 0`</span>
<span style="color:green; text-decoration:underline">`rifleflaktaperin1 0.0`</span>
<span style="color:green; text-decoration:underline">`rifleflaktaperin2 0.0`</span>
<span style="color:green; text-decoration:underline">`rifleflaktaperout1 0.0`</span>
<span style="color:green; text-decoration:underline">`rifleflaktaperout2 0.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakteampenalty1 0.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakteampenalty2 0.0`</span>
<span style="color:green; text-decoration:underline">`rifleflaktorsodamage1 0.4`</span>
<span style="color:green; text-decoration:underline">`rifleflaktorsodamage2 0.4`</span>
<span style="color:green; text-decoration:underline">`rifleflakvisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakvisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakvistime1 0`</span>
<span style="color:green; text-decoration:underline">`rifleflakvistime2 0`</span>
<span style="color:green; text-decoration:underline">`rifleflakwaterfric1 2.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakwaterfric2 2.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakwavepush1 1.5`</span>
<span style="color:green; text-decoration:underline">`rifleflakwavepush2 1.5`</span>
<span style="color:green; text-decoration:underline">`rifleflakweight1 0.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakweight2 0.0`</span>
<span style="color:green; text-decoration:underline">`rifleflakwhipdamage1 0.6`</span>
<span style="color:green; text-decoration:underline">`rifleflakwhipdamage2 0.6`</span>
<span style="color:green; text-decoration:underline">`riflefragdelay1 0`</span>
<span style="color:green; text-decoration:underline">`riflefragdelay2 0`</span>
<span style="color:green; text-decoration:underline">`riflefragjump1 0.0`</span>
<span style="color:green; text-decoration:underline">`riflefragjump2 0.0`</span>
<span style="color:green; text-decoration:underline">`riflefragoffset1 1.0`</span>
<span style="color:green; text-decoration:underline">`riflefragoffset2 1.0`</span>
<span style="color:green; text-decoration:underline">`riflefragrays1`</span>` 5`
<span style="color:red; text-decoration:line-through">`rifleflakrays2`</span><span style="color:green; text-decoration:underline">`riflefragrays2`</span>` 5`
<span style="color:red; text-decoration:line-through">`rifleflakrel1`</span><span style="color:green; text-decoration:underline">`riflefragrel1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`rifleflakrel2`</span><span style="color:green; text-decoration:underline">`riflefragrel2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`rifleflakscale1`</span><span style="color:green; text-decoration:underline">`riflefragscale1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`rifleflakscale2`</span><span style="color:green; text-decoration:underline">`riflefragscale2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`rifleflakskew1`</span><span style="color:green; text-decoration:underline">`riflefragskew1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`rifleflakskew2`</span><span style="color:green; text-decoration:underline">`riflefragskew2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`rifleflakspeed1`</span><span style="color:green; text-decoration:underline">`riflefragspeed1`</span>` 0`
<span style="color:red; text-decoration:line-through">`rifleflakspeed2`</span><span style="color:green; text-decoration:underline">`riflefragspeed2`</span>` 0`
<span style="color:red; text-decoration:line-through">`rifleflakspread1`</span><span style="color:green; text-decoration:underline">`riflefragspread1`</span>` 0.25`
<span style="color:red; text-decoration:line-through">`rifleflakspread2`</span><span style="color:green; text-decoration:underline">`riflefragspread2`</span>` 0.25`
<span style="color:red; text-decoration:line-through">`rifleflaktime1`</span><span style="color:green; text-decoration:underline">`riflefragtime1`</span>` 500`
<span style="color:red; text-decoration:line-through">`rifleflaktime2`</span><span style="color:green; text-decoration:underline">`riflefragtime2`</span>` 500`
<span style="color:red; text-decoration:line-through">`rifleflakweap1`</span><span style="color:green; text-decoration:underline">`riflefragweap1`</span>` -1`
<span style="color:red; text-decoration:line-through">`rifleflakweap2`</span><span style="color:green; text-decoration:underline">`riflefragweap2`</span>` -1`
`riflefrequency 1.0`
`riflefullauto1 0`
`riflefullauto2 0`
<span style="color:red; text-decoration:line-through">`riflegdelay1 0`</span>
<span style="color:red; text-decoration:line-through">`riflegdelay2 0`</span>
`rifleguided1 0`
`rifleguided2 0`
<span style="color:green; text-decoration:underline">`rifleguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`rifleguideddelay2 0`</span>
`rifleheadmin1 4.0`
`rifleheadmin2 4.0`
`riflehitpush1 `<span style="color:red; text-decoration:line-through">`50.0`</span><span style="color:green; text-decoration:underline">`25.0`</span>
`riflehitpush2 100.0`
<span style="color:red; text-decoration:line-through">`riflejamchance 75`</span><span style="color:green; text-decoration:underline">`rifleinteracts1 1`</span>
<span style="color:green; text-decoration:underline">`rifleinteracts2 1`</span>
`riflekickpush1 `<span style="color:red; text-decoration:line-through">`50.0`</span><span style="color:green; text-decoration:underline">`35.0`</span>
`riflekickpush2 50.0`
`riflelaser 0`
<span style="color:red; text-decoration:line-through">`riflelegsdmg1 0.3`</span><span style="color:green; text-decoration:underline">`riflelegdamage1 0.2`</span>
<span style="color:red; text-decoration:line-through">`riflelegsdmg2 0.3`</span><span style="color:green; text-decoration:underline">`riflelegdamage2 0.2`</span>
`riflelimspeed1 0`
`riflelimspeed2 0`
`riflemax `<span style="color:red; text-decoration:line-through">`5`</span>
<span style="color:red; text-decoration:line-through">`riflemaxspread1 0`</span>
<span style="color:red; text-decoration:line-through">`riflemaxspread2 0`</span><span style="color:green; text-decoration:underline">`6`</span>
`rifleminspeed1 0.0`
`rifleminspeed2 0.0`
<span style="color:red; text-decoration:line-through">`rifleminspread1 0`</span><span style="color:green; text-decoration:underline">`riflemodes -64`</span>
<span style="color:red; text-decoration:line-through">`rifleminspread2 0`</span><span style="color:green; text-decoration:underline">`riflemuts -56`</span>
`riflename "rifle"`
`riflepartcol1 `<span style="color:red; text-decoration:line-through">`0x8822DD`</span><span style="color:green; text-decoration:underline">`0xA020F0`</span>
`riflepartcol2 `<span style="color:red; text-decoration:line-through">`0x8822DD`</span><span style="color:green; text-decoration:underline">`0xA020F0`</span>
`riflepartlen1 256.0`
`riflepartlen2 `<span style="color:red; text-decoration:line-through">`512.0`</span><span style="color:green; text-decoration:underline">`1024.0`</span>
`riflepartsize1 `<span style="color:red; text-decoration:line-through">`1.5`</span><span style="color:green; text-decoration:underline">`2.0`</span>
`riflepartsize2 3.0`
`rifleparttype1 7`
`rifleparttype2 7`
<span style="color:red; text-decoration:line-through">`riflepdelay1 0`</span>
<span style="color:red; text-decoration:line-through">`riflepdelay2 0`</span>
`riflepower1 0`
`riflepower2 0`
<span style="color:red; text-decoration:line-through">`riflepusharea 1.5`</span><span style="color:green; text-decoration:underline">`rifleprojdelay1 0`</span>
<span style="color:green; text-decoration:underline">`rifleprojdelay2 0`</span>
<span style="color:green; text-decoration:underline">`rifleproxdelay1 0`</span>
<span style="color:green; text-decoration:underline">`rifleproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`rifleproxdist1 0.0`</span>
<span style="color:green; text-decoration:underline">`rifleproxdist2 0.0`</span>
<span style="color:green; text-decoration:underline">`rifleproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`rifleproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`rifleproxtype1 0`</span>
<span style="color:green; text-decoration:underline">`rifleproxtype2 0`</span>
`rifleradial1 0`
`rifleradial2 0`
`rifleradius1 1.0`
`rifleradius2 1.0`
`riflerays1 1`
`riflerays2 1`
<span style="color:red; text-decoration:line-through">`riflerdelay 1750`</span>
`riflereflectivity1 0.0`
`riflereflectivity2 0.0`
`riflerelativity1 1.0`
`riflerelativity2 0.0`
<span style="color:green; text-decoration:underline">`riflereloaddelay 2500`</span>
`riflereloads -1`
`rifleresidual1 0`
`rifleresidual2 0`
<span style="color:red; text-decoration:line-through">`rifleselfdmg1`</span><span style="color:green; text-decoration:underline">`rifleselfdamage1`</span>` 0.5`
<span style="color:red; text-decoration:line-through">`rifleselfdmg2`</span><span style="color:green; text-decoration:underline">`rifleselfdamage2`</span>` 0.5 `<span style="color:red; text-decoration:line-through">`rifleslow1 0.0`</span>
<span style="color:red; text-decoration:line-through">`rifleslow2 0.0`</span>
`riflespeed1 10000`
`riflespeed2 100000`
`riflespread1 `<span style="color:red; text-decoration:line-through">`1`</span><span style="color:green; text-decoration:underline">`0.1`</span>
`riflespread2 `<span style="color:red; text-decoration:line-through">`0`</span><span style="color:green; text-decoration:underline">`0.0`</span>
<span style="color:green; text-decoration:underline">`riflespreadmax1 0.0`</span>
<span style="color:green; text-decoration:underline">`riflespreadmax2 0.0`</span>
<span style="color:green; text-decoration:underline">`riflespreadmin1 0.0`</span>
<span style="color:green; text-decoration:underline">`riflespreadmin2 0.0`</span>
<span style="color:green; text-decoration:underline">`riflespreadz1 1.0`</span>
<span style="color:green; text-decoration:underline">`riflespreadz2 1.0`</span>
<span style="color:green; text-decoration:underline">`riflestunfall1 0.0`</span>
<span style="color:green; text-decoration:underline">`riflestunfall2 0.0`</span>
`riflestunscale1 0.5`
`riflestunscale2 1.0`
`riflestuntime1 `<span style="color:red; text-decoration:line-through">`100`</span><span style="color:green; text-decoration:underline">`75`</span>
`riflestuntime2 200`
`riflesub1 1`
`riflesub2 1`
<span style="color:green; text-decoration:underline">`rifletaper1 0`</span>
<span style="color:green; text-decoration:underline">`rifletaper2 0`</span>
`rifletaperin1 0.0`
`rifletaperin2 0.0`
`rifletaperout1 0.0`
`rifletaperout2 0.0`
<span style="color:green; text-decoration:underline">`rifleteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`rifleteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`rifleteampenalty1 1.0`</span>
<span style="color:green; text-decoration:underline">`rifleteampenalty2 1.0`</span>
`rifletime1 5000`
`rifletime2 5000`
<span style="color:red; text-decoration:line-through">`rifletorsodmg1 0.5`</span><span style="color:green; text-decoration:underline">`rifletorsodamage1 0.4`</span>
<span style="color:red; text-decoration:line-through">`rifletorsodmg2 0.5`</span><span style="color:green; text-decoration:underline">`rifletorsodamage2 0.4`</span>
`rifletrace1 1.0`
`rifletrace2 1.0`
<span style="color:green; text-decoration:underline">`riflevisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`riflevisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`riflevistime1 0`</span>
<span style="color:green; text-decoration:underline">`riflevistime2 0`</span>
`riflewaterfric1 2.0`
`riflewaterfric2 2.0`
<span style="color:green; text-decoration:underline">`riflewavepush1 1.5`</span>
<span style="color:green; text-decoration:underline">`riflewavepush2 1.5`</span>
`rifleweight1 0.0`
`rifleweight2 0.0`
<span style="color:red; text-decoration:line-through">`riflewhipdmg1 0.75`</span><span style="color:green; text-decoration:underline">`riflewhipdamage1 0.6`</span>
<span style="color:red; text-decoration:line-through">`riflewhipdmg2 0.75`</span>
<span style="color:red; text-decoration:line-through">`riflezdiv1 0`</span>
<span style="color:red; text-decoration:line-through">`riflezdiv2 0`</span><span style="color:green; text-decoration:underline">`riflewhipdamage2 0.6`</span>
`riflezooms 1`
`rocketadd 1`
<span style="color:red; text-decoration:line-through">`rocketadelay1 1000`</span>
<span style="color:red; text-decoration:line-through">`rocketadelay2 1000`</span>
`rocketaidist1 1024.0`
`rocketaidist2 512.0`
`rocketaiskew1 10`
`rocketaiskew2 10`
<span style="color:red; text-decoration:line-through">`rocketallowed 3`</span><span style="color:green; text-decoration:underline">`rocketattackdelay1 1500`</span>
<span style="color:green; text-decoration:underline">`rocketattackdelay2 1500`</span>
`rocketcarried 1`
`rocketcollide1 `<span style="color:red; text-decoration:line-through">`597`</span><span style="color:green; text-decoration:underline">`62`</span>
`rocketcollide2 `<span style="color:red; text-decoration:line-through">`597`</span><span style="color:green; text-decoration:underline">`62`</span>
`rocketcolour `<span style="color:red; text-decoration:line-through">`0xAA3300`</span><span style="color:green; text-decoration:underline">`0x803000`</span>
`rocketcooked1 8`
`rocketcooked2 8`
<span style="color:red; text-decoration:line-through">`rocketcritdash1 0`</span>
<span style="color:red; text-decoration:line-through">`rocketcritdash2 0`</span>
<span style="color:red; text-decoration:line-through">`rocketcritdist 0.0`</span>
<span style="color:red; text-decoration:line-through">`rocketcritmult 2.0`</span>
`rocketdamage2 `<span style="color:red; text-decoration:line-through">`150`</span><span style="color:green; text-decoration:underline">`200`</span>
`rocketdelta1 10.0`
`rocketdelta2 10.0`
<span style="color:red; text-decoration:line-through">`rocketedelay1 200`</span><span style="color:green; text-decoration:underline">`rocketdrill1 0`</span>
<span style="color:red; text-decoration:line-through">`rocketedelay2 200`</span><span style="color:green; text-decoration:underline">`rocketdrill2 0`</span>
`rocketelasticity1 0.5`
`rocketelasticity2 0.5`
<span style="color:green; text-decoration:underline">`rocketescapedelay1 200`</span>
<span style="color:green; text-decoration:underline">`rocketescapedelay2 200`</span>
`rocketexplcol1 0x981808`
`rocketexplcol2 0x981808`
`rocketexplode1 `<span style="color:red; text-decoration:line-through">`100`</span><span style="color:green; text-decoration:underline">`128.0`</span>
`rocketexplode2 `<span style="color:red; text-decoration:line-through">`100`</span><span style="color:green; text-decoration:underline">`128.0`</span>
`rocketextinguish1 2`
`rocketextinguish2 2`
`rocketflakcollide1 `<span style="color:red; text-decoration:line-through">`597`</span><span style="color:green; text-decoration:underline">`62`</span>
`rocketflakcollide2 `<span style="color:red; text-decoration:line-through">`597`</span><span style="color:green; text-decoration:underline">`62`</span>
<span style="color:red; text-decoration:line-through">`rocketflakdmg1 300`</span><span style="color:green; text-decoration:underline">`rocketflakdamage1 200`</span>
<span style="color:red; text-decoration:line-through">`rocketflakdmg2 300`</span><span style="color:green; text-decoration:underline">`rocketflakdamage2 200`</span>
<span style="color:red; text-decoration:line-through">`rocketflakffwd1`</span><span style="color:green; text-decoration:underline">`rocketflakdelta1 10.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakdelta2 10.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakdrill1 0`</span>
<span style="color:green; text-decoration:underline">`rocketflakdrill2 0`</span>
<span style="color:green; text-decoration:underline">`rocketflakelasticity1 0.5`</span>
<span style="color:green; text-decoration:underline">`rocketflakelasticity2 0.5`</span>
<span style="color:green; text-decoration:underline">`rocketflakexplcol1 0x981808`</span>
<span style="color:green; text-decoration:underline">`rocketflakexplcol2 0x981808`</span>
<span style="color:green; text-decoration:underline">`rocketflakexplode1 128.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakexplode2 128.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakextinguish1 2`</span>
<span style="color:green; text-decoration:underline">`rocketflakextinguish2 2`</span>
<span style="color:green; text-decoration:underline">`rocketflakguided1 0`</span>
<span style="color:green; text-decoration:underline">`rocketflakguided2 1`</span>
<span style="color:green; text-decoration:underline">`rocketflakguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`rocketflakguideddelay2 0`</span>
<span style="color:green; text-decoration:underline">`rocketflakheadmin1 16.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakheadmin2 16.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakhitpush1 500.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakhitpush2 500.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakinteracts1 1`</span>
<span style="color:green; text-decoration:underline">`rocketflakinteracts2 1`</span>
<span style="color:green; text-decoration:underline">`rocketflaklegdamage1 0.2`</span>
<span style="color:green; text-decoration:underline">`rocketflaklegdamage2 0.2`</span>
<span style="color:green; text-decoration:underline">`rocketflakminspeed1 50.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakminspeed2 50.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakpartcol1 -1`</span>
<span style="color:green; text-decoration:underline">`rocketflakpartcol2 -1`</span>
<span style="color:green; text-decoration:underline">`rocketflakpartlen1`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`rocketflakffwd2`</span><span style="color:green; text-decoration:underline">`rocketflakpartlen2`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`rocketflakminspeed1`</span><span style="color:green; text-decoration:underline">`rocketflakpartsize1 3.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakpartsize2 3.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakparttype1 10`</span>
<span style="color:green; text-decoration:underline">`rocketflakparttype2 10`</span>
<span style="color:green; text-decoration:underline">`rocketflakproxdelay1 0`</span>
<span style="color:green; text-decoration:underline">`rocketflakproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`rocketflakproxdist1`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`rocketflakminspeed2`</span><span style="color:green; text-decoration:underline">`rocketflakproxdist2 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`rocketflakproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`rocketflakproxtype1 0`</span>
<span style="color:green; text-decoration:underline">`rocketflakproxtype2 0`</span>
<span style="color:green; text-decoration:underline">`rocketflakradial1 0`</span>
<span style="color:green; text-decoration:underline">`rocketflakradial2 0`</span>
<span style="color:green; text-decoration:underline">`rocketflakradius1 1.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakradius2 1.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakreflectivity1 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakreflectivity2`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`rocketflakoffset1`</span><span style="color:green; text-decoration:underline">`rocketflakresidual1 1`</span>
<span style="color:green; text-decoration:underline">`rocketflakresidual2 1`</span>
<span style="color:green; text-decoration:underline">`rocketflakselfdamage1 0.5`</span>
<span style="color:green; text-decoration:underline">`rocketflakselfdamage2 0.5`</span>
<span style="color:green; text-decoration:underline">`rocketflakstunfall1 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakstunfall2 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakstunscale1 4.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakstunscale2 4.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakstuntime1 500`</span>
<span style="color:green; text-decoration:underline">`rocketflakstuntime2 500`</span>
<span style="color:green; text-decoration:underline">`rocketflaktaper1 0`</span>
<span style="color:green; text-decoration:underline">`rocketflaktaper2 0`</span>
<span style="color:green; text-decoration:underline">`rocketflaktaperin1 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketflaktaperin2 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketflaktaperout1 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketflaktaperout2 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakteampenalty1`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`rocketflakoffset2`</span><span style="color:green; text-decoration:underline">`rocketflakteampenalty2`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`rocketflakrays1 75`</span><span style="color:green; text-decoration:underline">`rocketflaktorsodamage1 0.4`</span>
<span style="color:green; text-decoration:underline">`rocketflaktorsodamage2 0.4`</span>
<span style="color:green; text-decoration:underline">`rocketflakvisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakvisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakvistime1 0`</span>
<span style="color:green; text-decoration:underline">`rocketflakvistime2 0`</span>
<span style="color:green; text-decoration:underline">`rocketflakwaterfric1 2.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakwaterfric2 2.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakwavepush1 4.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakwavepush2 4.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakweight1 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakweight2 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketflakwhipdamage1 0.6`</span>
<span style="color:green; text-decoration:underline">`rocketflakwhipdamage2 0.6`</span>
<span style="color:green; text-decoration:underline">`rocketfragdelay1 3`</span>
<span style="color:green; text-decoration:underline">`rocketfragdelay2 3`</span>
<span style="color:green; text-decoration:underline">`rocketfragjump1 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketfragjump2 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketfragoffset1 2.0`</span>
<span style="color:green; text-decoration:underline">`rocketfragoffset2 2.0`</span>
<span style="color:green; text-decoration:underline">`rocketfragrays1 30`</span>
<span style="color:red; text-decoration:line-through">`rocketflakrays2 75`</span><span style="color:green; text-decoration:underline">`rocketfragrays2 30`</span>
<span style="color:red; text-decoration:line-through">`rocketflakrel1`</span><span style="color:green; text-decoration:underline">`rocketfragrel1`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`rocketflakrel2`</span><span style="color:green; text-decoration:underline">`rocketfragrel2`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`rocketflakscale1`</span><span style="color:green; text-decoration:underline">`rocketfragscale1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`rocketflakscale2`</span><span style="color:green; text-decoration:underline">`rocketfragscale2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`rocketflakskew1`</span><span style="color:green; text-decoration:underline">`rocketfragskew1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`rocketflakskew2`</span><span style="color:green; text-decoration:underline">`rocketfragskew2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`rocketflakspeed1`</span><span style="color:green; text-decoration:underline">`rocketfragspeed1`</span>` 400`
<span style="color:red; text-decoration:line-through">`rocketflakspeed2`</span><span style="color:green; text-decoration:underline">`rocketfragspeed2`</span>` 400`
<span style="color:red; text-decoration:line-through">`rocketflakspread1`</span><span style="color:green; text-decoration:underline">`rocketfragspread1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`rocketflakspread2`</span><span style="color:green; text-decoration:underline">`rocketfragspread2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`rocketflaktime1 3000`</span><span style="color:green; text-decoration:underline">`rocketfragtime1 1000`</span>
<span style="color:red; text-decoration:line-through">`rocketflaktime2 3000`</span><span style="color:green; text-decoration:underline">`rocketfragtime2 1000`</span>
<span style="color:red; text-decoration:line-through">`rocketflakweap1`</span><span style="color:green; text-decoration:underline">`rocketfragweap1`</span>` 4`
<span style="color:red; text-decoration:line-through">`rocketflakweap2`</span><span style="color:green; text-decoration:underline">`rocketfragweap2`</span>` 4`
`rocketfrequency 4.0`
`rocketfullauto1 0`
`rocketfullauto2 0`
<span style="color:red; text-decoration:line-through">`rocketgdelay1 0`</span>
<span style="color:red; text-decoration:line-through">`rocketgdelay2 0`</span>
`rocketguided1 0`
`rocketguided2 1`
<span style="color:green; text-decoration:underline">`rocketguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`rocketguideddelay2 0`</span>
`rocketheadmin1 16.0`
`rocketheadmin2 16.0`
`rockethitpush1 500.0`
`rockethitpush2 500.0`
<span style="color:red; text-decoration:line-through">`rocketjamchance 50`</span><span style="color:green; text-decoration:underline">`rocketinteracts1 1`</span>
<span style="color:green; text-decoration:underline">`rocketinteracts2 1`</span>
`rocketkickpush1 150.0`
`rocketkickpush2 150.0`
`rocketlaser 0`
<span style="color:red; text-decoration:line-through">`rocketlegsdmg1`</span><span style="color:green; text-decoration:underline">`rocketlegdamage1`</span>` 0.2`
<span style="color:red; text-decoration:line-through">`rocketlegsdmg2`</span><span style="color:green; text-decoration:underline">`rocketlegdamage2`</span>` 0.2`
`rocketlimspeed1 0`
`rocketlimspeed2 0`
`rocketmax 1`
<span style="color:red; text-decoration:line-through">`rocketmaxspread1 0`</span>
<span style="color:red; text-decoration:line-through">`rocketmaxspread2 0`</span>
`rocketminspeed1 0.0`
`rocketminspeed2 0.0`
<span style="color:red; text-decoration:line-through">`rocketminspread1 0`</span><span style="color:green; text-decoration:underline">`rocketmodes -64`</span>
<span style="color:red; text-decoration:line-through">`rocketminspread2 0`</span><span style="color:green; text-decoration:underline">`rocketmuts -192`</span>
`rocketname "rocket"`
`rocketpartcol1 -1`
`rocketpartcol2 -1`
`rocketpartlen2 0.0`
`rocketpartsize1 3.0`
`rocketpartsize2 3.0`
`rocketparttype1 `<span style="color:red; text-decoration:line-through">`9`</span><span style="color:green; text-decoration:underline">`10`</span>
`rocketparttype2 `<span style="color:red; text-decoration:line-through">`9`</span><span style="color:green; text-decoration:underline">`10`</span>
<span style="color:red; text-decoration:line-through">`rocketpdelay1`</span><span style="color:green; text-decoration:underline">`rocketpower1 3000`</span>
<span style="color:green; text-decoration:underline">`rocketpower2 3000`</span>
<span style="color:green; text-decoration:underline">`rocketprojdelay1`</span>` 0`
<span style="color:red; text-decoration:line-through">`rocketpdelay2`</span><span style="color:green; text-decoration:underline">`rocketprojdelay2`</span>` 0`
<span style="color:red; text-decoration:line-through">`rocketpower1 2000`</span><span style="color:green; text-decoration:underline">`rocketproxdelay1 0`</span>
<span style="color:red; text-decoration:line-through">`rocketpower2 2000`</span><span style="color:green; text-decoration:underline">`rocketproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`rocketproxdist1 0.0`</span>
<span style="color:red; text-decoration:line-through">`rocketpusharea 4.0`</span><span style="color:green; text-decoration:underline">`rocketproxdist2 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`rocketproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`rocketproxtype1 0`</span>
<span style="color:green; text-decoration:underline">`rocketproxtype2 0`</span>
`rocketradial1 0`
`rocketradial2 0`
`rocketradius1 1.0`
`rocketradius2 1.0`
`rocketrays1 1`
`rocketrays2 1`
<span style="color:red; text-decoration:line-through">`rocketrdelay 1500`</span>
`rocketreflectivity1 0.0`
`rocketreflectivity2 0.0`
`rocketrelativity1 0.0`
`rocketrelativity2 0.0`
<span style="color:green; text-decoration:underline">`rocketreloaddelay 5000`</span>
`rocketreloads 0`
`rocketresidual1 1`
`rocketresidual2 1`
<span style="color:red; text-decoration:line-through">`rocketselfdmg1`</span><span style="color:green; text-decoration:underline">`rocketselfdamage1`</span>` 0.5`
<span style="color:red; text-decoration:line-through">`rocketselfdmg2`</span><span style="color:green; text-decoration:underline">`rocketselfdamage2`</span>` 0.5 `<span style="color:red; text-decoration:line-through">`rocketslow1 0.0`</span>
<span style="color:red; text-decoration:line-through">`rocketslow2 0.0`</span>
`rocketspeed1 1000`
`rocketspeed2 250`
`rocketspread1 `<span style="color:red; text-decoration:line-through">`1`</span><span style="color:green; text-decoration:underline">`1.0`</span>
`rocketspread2 `<span style="color:red; text-decoration:line-through">`1`</span><span style="color:green; text-decoration:underline">`1.0`</span>
<span style="color:green; text-decoration:underline">`rocketspreadmax1 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketspreadmax2 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketspreadmin1 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketspreadmin2 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketspreadz1 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketspreadz2 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketstunfall1 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketstunfall2 0.0`</span>
`rocketstunscale1 4.0`
`rocketstunscale2 4.0`
`rocketstuntime1 `<span style="color:red; text-decoration:line-through">`350`</span><span style="color:green; text-decoration:underline">`500`</span>
`rocketstuntime2 `<span style="color:red; text-decoration:line-through">`350`</span><span style="color:green; text-decoration:underline">`500`</span>
`rocketsub1 1`
`rocketsub2 1`
<span style="color:green; text-decoration:underline">`rockettaper1 0`</span>
<span style="color:green; text-decoration:underline">`rockettaper2 0`</span>
`rockettaperin1 0.0`
`rockettaperin2 0.0`
`rockettaperout1 0.0`
`rockettaperout2 0.0`
<span style="color:green; text-decoration:underline">`rocketteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`rocketteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`rocketteampenalty1 0.0`</span>
<span style="color:green; text-decoration:underline">`rocketteampenalty2 0.0`</span>
`rockettime1 5000`
`rockettime2 5000`
<span style="color:red; text-decoration:line-through">`rockettorsodmg1`</span><span style="color:green; text-decoration:underline">`rockettorsodamage1`</span>` 0.4`
<span style="color:red; text-decoration:line-through">`rockettorsodmg2`</span><span style="color:green; text-decoration:underline">`rockettorsodamage2`</span>` 0.4`
`rockettrace1 1.0`
`rockettrace2 1.0`
<span style="color:green; text-decoration:underline">`rocketvisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`rocketvisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`rocketvistime1 0`</span>
<span style="color:green; text-decoration:underline">`rocketvistime2 0`</span>
`rocketwaterfric1 2.0`
`rocketwaterfric2 2.0`
<span style="color:green; text-decoration:underline">`rocketwavepush1 4.0`</span>
<span style="color:green; text-decoration:underline">`rocketwavepush2 4.0`</span>
`rocketweight1 0.0`
`rocketweight2 0.0`
<span style="color:red; text-decoration:line-through">`rocketwhipdmg1`</span><span style="color:green; text-decoration:underline">`rocketwhipdamage1`</span>` 0.6`
<span style="color:red; text-decoration:line-through">`rocketwhipdmg2`</span><span style="color:green; text-decoration:underline">`rocketwhipdamage2`</span>` 0.6 `<span style="color:red; text-decoration:line-through">`rocketzdiv1 0`</span>
<span style="color:red; text-decoration:line-through">`rocketzdiv2 0`</span>
`rocketzooms 0`
<span style="color:green; text-decoration:underline">`rotatemaps 2`</span>
<span style="color:green; text-decoration:underline">`rotatemapsfilter 2`</span>
<span style="color:green; text-decoration:underline">`rotatemode 1`</span>
<span style="color:green; text-decoration:underline">`rotatemodefilter 188`</span>
<span style="color:green; text-decoration:underline">`rotatemuts 3`</span>
<span style="color:green; text-decoration:underline">`rotatemutsfilter 126399`</span>
`selfdamage 1`
<span style="color:green; text-decoration:underline">`selfdamagescale 1.0`</span>
<span style="color:green; text-decoration:underline">`serverclients 16`</span>
<span style="color:green; text-decoration:underline">`serverdebug 0`</span>
<span style="color:green; text-decoration:underline">`serverdesc ""`</span>
<span style="color:green; text-decoration:underline">`servermotd ""`</span>
<span style="color:green; text-decoration:underline">`serveropen 3`</span>
<span style="color:green; text-decoration:underline">`shockdamage 3`</span>
<span style="color:green; text-decoration:underline">`shockdelay 1000`</span>
<span style="color:green; text-decoration:underline">`shockstunfall 0.1`</span>
<span style="color:green; text-decoration:underline">`shockstunscale 0.5`</span>
<span style="color:green; text-decoration:underline">`shockstuntime 1000`</span>
<span style="color:green; text-decoration:underline">`shocktime 5500`</span>
`shotgunadd 2`
<span style="color:red; text-decoration:line-through">`shotgunadelay1 500`</span>
<span style="color:red; text-decoration:line-through">`shotgunadelay2 900`</span>
`shotgunaidist1 256.0`
`shotgunaidist2 512.0`
`shotgunaiskew1 10`
`shotgunaiskew2 10`
<span style="color:red; text-decoration:line-through">`shotgunallowed 2`</span><span style="color:green; text-decoration:underline">`shotgunattackdelay1 600`</span>
<span style="color:green; text-decoration:underline">`shotgunattackdelay2 1125`</span>
`shotguncarried 1`
`shotguncollide1 `<span style="color:red; text-decoration:line-through">`118`</span><span style="color:green; text-decoration:underline">`629`</span>
`shotguncollide2 `<span style="color:red; text-decoration:line-through">`117`</span><span style="color:green; text-decoration:underline">`61`</span>
`shotguncolour `<span style="color:red; text-decoration:line-through">`0x999900`</span><span style="color:green; text-decoration:underline">`0xF0F020`</span>
`shotguncooked1 0`
`shotguncooked2 0`
<span style="color:red; text-decoration:line-through">`shotguncritboost 2.0`</span>
<span style="color:red; text-decoration:line-through">`shotguncritdash1 0`</span>
<span style="color:red; text-decoration:line-through">`shotguncritdash2 0`</span>
<span style="color:red; text-decoration:line-through">`shotguncritdist 256.0`</span>
<span style="color:red; text-decoration:line-through">`shotguncritmult 2.0`</span>
`shotgundamage1 15`
`shotgundamage2 4`
`shotgundelta1 10.0`
`shotgundelta2 10.0`
<span style="color:red; text-decoration:line-through">`shotgunedelay1 200`</span><span style="color:green; text-decoration:underline">`shotgundrill1 2`</span>
<span style="color:red; text-decoration:line-through">`shotgunedelay2 200`</span><span style="color:green; text-decoration:underline">`shotgundrill2 0`</span>
`shotgunelasticity1 0.5`
`shotgunelasticity2 0.5`
<span style="color:green; text-decoration:underline">`shotgunescapedelay1 200`</span>
<span style="color:green; text-decoration:underline">`shotgunescapedelay2 200`</span>
`shotgunexplcol2 `<span style="color:red; text-decoration:line-through">`0x999900`</span><span style="color:green; text-decoration:underline">`0xF0F020`</span>
`shotgunexplode1 `<span style="color:red; text-decoration:line-through">`0`</span><span style="color:green; text-decoration:underline">`0.0`</span>
`shotgunexplode2 `<span style="color:red; text-decoration:line-through">`0`</span><span style="color:green; text-decoration:underline">`0.0`</span>
`shotgunextinguish1 2`
`shotgunextinguish2 2`
`shotgunflakcollide1 `<span style="color:red; text-decoration:line-through">`118`</span><span style="color:green; text-decoration:underline">`117`</span>
`shotgunflakcollide2 `<span style="color:red; text-decoration:line-through">`118`</span><span style="color:green; text-decoration:underline">`117`</span>
<span style="color:red; text-decoration:line-through">`shotgunflakdmg1 16`</span><span style="color:green; text-decoration:underline">`shotgunflakdamage1 15`</span>
<span style="color:red; text-decoration:line-through">`shotgunflakdmg2 4`</span><span style="color:green; text-decoration:underline">`shotgunflakdamage2 8`</span>
<span style="color:red; text-decoration:line-through">`shotgunflakffwd1`</span><span style="color:green; text-decoration:underline">`shotgunflakdelta1 10.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakdelta2 10.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakdrill1 2`</span>
<span style="color:green; text-decoration:underline">`shotgunflakdrill2 0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakelasticity1 0.5`</span>
<span style="color:green; text-decoration:underline">`shotgunflakelasticity2 0.5`</span>
<span style="color:green; text-decoration:underline">`shotgunflakexplcol1 0xF0F020`</span>
<span style="color:green; text-decoration:underline">`shotgunflakexplcol2 0xF0F020`</span>
<span style="color:green; text-decoration:underline">`shotgunflakexplode1`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`shotgunflakffwd2`</span><span style="color:green; text-decoration:underline">`shotgunflakexplode2`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`shotgunflakminspeed1`</span><span style="color:green; text-decoration:underline">`shotgunflakextinguish1 2`</span>
<span style="color:green; text-decoration:underline">`shotgunflakextinguish2 2`</span>
<span style="color:green; text-decoration:underline">`shotgunflakguided1 0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakguided2 0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakguideddelay2 0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakheadmin1 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakheadmin2 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakhitpush1 50.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakhitpush2`</span>` 25.0`
<span style="color:green; text-decoration:underline">`shotgunflakinteracts1 1`</span>
<span style="color:green; text-decoration:underline">`shotgunflakinteracts2 3`</span>
<span style="color:green; text-decoration:underline">`shotgunflaklegdamage1 0.3`</span>
<span style="color:green; text-decoration:underline">`shotgunflaklegdamage2 0.3`</span>
<span style="color:green; text-decoration:underline">`shotgunflakminspeed1 50.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakpartcol1 0xF0F020`</span>
<span style="color:green; text-decoration:underline">`shotgunflakpartcol2 0xF0F020`</span>
<span style="color:green; text-decoration:underline">`shotgunflakpartlen1 7.5`</span>
<span style="color:green; text-decoration:underline">`shotgunflakpartlen2 7.5`</span>
<span style="color:green; text-decoration:underline">`shotgunflakpartsize1 0.35`</span>
<span style="color:green; text-decoration:underline">`shotgunflakpartsize2 0.35`</span>
<span style="color:green; text-decoration:underline">`shotgunflakparttype1 3`</span>
<span style="color:green; text-decoration:underline">`shotgunflakparttype2 3`</span>
<span style="color:green; text-decoration:underline">`shotgunflakproxdelay1 0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakproxdist1 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakproxdist2 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakproxtype1 0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakproxtype2 0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakradial1 0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakradial2 0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakradius1 1.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakradius2 1.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakreflectivity1 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakreflectivity2 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakresidual1 0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakresidual2 2`</span>
<span style="color:green; text-decoration:underline">`shotgunflakselfdamage1 0.5`</span>
<span style="color:green; text-decoration:underline">`shotgunflakselfdamage2 0.5`</span>
<span style="color:green; text-decoration:underline">`shotgunflakstunfall1 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakstunfall2 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakstunscale1 1.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakstunscale2 0.5`</span>
<span style="color:green; text-decoration:underline">`shotgunflakstuntime1 100`</span>
<span style="color:green; text-decoration:underline">`shotgunflakstuntime2 100`</span>
<span style="color:green; text-decoration:underline">`shotgunflaktaper1 0`</span>
<span style="color:green; text-decoration:underline">`shotgunflaktaper2 0`</span>
<span style="color:green; text-decoration:underline">`shotgunflaktaperin1 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflaktaperin2 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflaktaperout1 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflaktaperout2 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakteampenalty1 1.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakteampenalty2 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflaktorsodamage1 0.6`</span>
<span style="color:green; text-decoration:underline">`shotgunflaktorsodamage2 0.6`</span>
<span style="color:green; text-decoration:underline">`shotgunflakvisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakvisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakvistime1 0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakvistime2 0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakwaterfric1 2.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakwaterfric2 2.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakwavepush1 1.5`</span>
<span style="color:green; text-decoration:underline">`shotgunflakwavepush2 1.5`</span>
<span style="color:green; text-decoration:underline">`shotgunflakweight1 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakweight2 250.0`</span>
<span style="color:green; text-decoration:underline">`shotgunflakwhipdamage1 0.8`</span>
<span style="color:green; text-decoration:underline">`shotgunflakwhipdamage2 0.8`</span>
<span style="color:green; text-decoration:underline">`shotgunfragdelay1 0`</span>
<span style="color:green; text-decoration:underline">`shotgunfragdelay2 0`</span>
<span style="color:green; text-decoration:underline">`shotgunfragjump1 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunfragjump2 0.0`</span>
<span style="color:red; text-decoration:line-through">`shotgunflakoffset1 8.0`</span><span style="color:green; text-decoration:underline">`shotgunfragoffset1 4.0`</span>
<span style="color:red; text-decoration:line-through">`shotgunflakoffset2 8.0`</span><span style="color:green; text-decoration:underline">`shotgunfragoffset2 4.0`</span>
<span style="color:red; text-decoration:line-through">`shotgunflakrays1`</span><span style="color:green; text-decoration:underline">`shotgunfragrays1`</span>` 5`
<span style="color:red; text-decoration:line-through">`shotgunflakrays2 40`</span><span style="color:green; text-decoration:underline">`shotgunfragrays2 20`</span>
<span style="color:red; text-decoration:line-through">`shotgunflakrel1`</span><span style="color:green; text-decoration:underline">`shotgunfragrel1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`shotgunflakrel2`</span><span style="color:green; text-decoration:underline">`shotgunfragrel2`</span>` 1.5`
<span style="color:red; text-decoration:line-through">`shotgunflakscale1`</span><span style="color:green; text-decoration:underline">`shotgunfragscale1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`shotgunflakscale2`</span><span style="color:green; text-decoration:underline">`shotgunfragscale2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`shotgunflakskew1`</span><span style="color:green; text-decoration:underline">`shotgunfragskew1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`shotgunflakskew2`</span><span style="color:green; text-decoration:underline">`shotgunfragskew2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`shotgunflakspeed1`</span><span style="color:green; text-decoration:underline">`shotgunfragspeed1`</span>` 0`
<span style="color:red; text-decoration:line-through">`shotgunflakspeed2`</span><span style="color:green; text-decoration:underline">`shotgunfragspeed2`</span>` 0`
<span style="color:red; text-decoration:line-through">`shotgunflakspread1`</span><span style="color:green; text-decoration:underline">`shotgunfragspread1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`shotgunflakspread2`</span><span style="color:green; text-decoration:underline">`shotgunfragspread2`</span>` 0.2`
<span style="color:red; text-decoration:line-through">`shotgunflaktime1`</span><span style="color:green; text-decoration:underline">`shotgunfragtime1`</span>` 250`
<span style="color:red; text-decoration:line-through">`shotgunflaktime2`</span><span style="color:green; text-decoration:underline">`shotgunfragtime2`</span>` 2000`
<span style="color:red; text-decoration:line-through">`shotgunflakweap1`</span><span style="color:green; text-decoration:underline">`shotgunfragweap1`</span>` -1`
<span style="color:red; text-decoration:line-through">`shotgunflakweap2 13`</span><span style="color:green; text-decoration:underline">`shotgunfragweap2 14`</span>
`shotgunfrequency 1.0`
`shotgunfullauto1 0`
`shotgunfullauto2 0`
<span style="color:red; text-decoration:line-through">`shotgungdelay1 0`</span>
<span style="color:red; text-decoration:line-through">`shotgungdelay2 0`</span>
`shotgunguided1 0`
`shotgunguided2 0`
<span style="color:green; text-decoration:underline">`shotgunguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`shotgunguideddelay2 0`</span>
`shotgunheadmin1 0.0`
`shotgunheadmin2 0.0`
`shotgunhitpush1 50.0`
`shotgunhitpush2 25.0`
<span style="color:red; text-decoration:line-through">`shotgunjamchance 100`</span><span style="color:green; text-decoration:underline">`shotguninteracts1 1`</span>
<span style="color:green; text-decoration:underline">`shotguninteracts2 3`</span>
`shotgunkickpush1 50.0`
`shotgunkickpush2 75.0`
`shotgunlaser 0`
<span style="color:red; text-decoration:line-through">`shotgunlegsdmg1`</span><span style="color:green; text-decoration:underline">`shotgunlegdamage1`</span>` 0.3`
<span style="color:red; text-decoration:line-through">`shotgunlegsdmg2 0.4`</span><span style="color:green; text-decoration:underline">`shotgunlegdamage2 0.3`</span>
`shotgunlimspeed1 0`
`shotgunlimspeed2 0`
`shotgunmax `<span style="color:red; text-decoration:line-through">`8`</span>
<span style="color:red; text-decoration:line-through">`shotgunmaxspread1 0`</span>
<span style="color:red; text-decoration:line-through">`shotgunmaxspread2 0`</span><span style="color:green; text-decoration:underline">`10`</span>
`shotgunminspeed1 25.0`
`shotgunminspeed2 25.0`
<span style="color:red; text-decoration:line-through">`shotgunminspread1 16`</span><span style="color:green; text-decoration:underline">`shotgunmodes -64`</span>
<span style="color:red; text-decoration:line-through">`shotgunminspread2 0`</span><span style="color:green; text-decoration:underline">`shotgunmuts -56`</span>
`shotgunname "shotgun"`
`shotgunpartcol1 `<span style="color:red; text-decoration:line-through">`0x999900`</span><span style="color:green; text-decoration:underline">`0xF0F020`</span>
`shotgunpartcol2 `<span style="color:red; text-decoration:line-through">`0x999900`</span><span style="color:green; text-decoration:underline">`0xF0F020`</span>
`shotgunpartlen1 25.0`
`shotgunpartlen2 15.0`
`shotgunpartsize1 0.65`
`shotgunpartsize2 0.45`
`shotgunparttype1 3`
`shotgunparttype2 3`
<span style="color:red; text-decoration:line-through">`shotgunpdelay1 0`</span>
<span style="color:red; text-decoration:line-through">`shotgunpdelay2 0`</span>
`shotgunpower1 0`
`shotgunpower2 0`
<span style="color:red; text-decoration:line-through">`shotgunpusharea 1.5`</span><span style="color:green; text-decoration:underline">`shotgunprojdelay1 0`</span>
<span style="color:green; text-decoration:underline">`shotgunprojdelay2 0`</span>
<span style="color:green; text-decoration:underline">`shotgunproxdelay1 0`</span>
<span style="color:green; text-decoration:underline">`shotgunproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`shotgunproxdist1 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunproxdist2 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`shotgunproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`shotgunproxtype1 0`</span>
<span style="color:green; text-decoration:underline">`shotgunproxtype2 0`</span>
`shotgunradial1 0`
`shotgunradial2 0`
`shotgunradius1 1.0`
`shotgunradius2 1.0`
`shotgunrays1 10`
`shotgunrays2 1`
<span style="color:red; text-decoration:line-through">`shotgunrdelay 750`</span>
`shotgunreflectivity1 0.0`
`shotgunreflectivity2 0.0`
`shotgunrelativity1 0.05`
`shotgunrelativity2 0.75`
<span style="color:green; text-decoration:underline">`shotgunreloaddelay 750`</span>
`shotgunreloads -1`
`shotgunresidual1 0`
`shotgunresidual2 2`
<span style="color:red; text-decoration:line-through">`shotgunselfdmg1`</span><span style="color:green; text-decoration:underline">`shotgunselfdamage1`</span>` 0.5`
<span style="color:red; text-decoration:line-through">`shotgunselfdmg2`</span><span style="color:green; text-decoration:underline">`shotgunselfdamage2`</span>` 0.5 `<span style="color:red; text-decoration:line-through">`shotgunslow1 0.0`</span>
<span style="color:red; text-decoration:line-through">`shotgunslow2 0.0`</span>
`shotgunspeed1 1250`
`shotgunspeed2 250`
`shotgunspread1 `<span style="color:red; text-decoration:line-through">`4`</span><span style="color:green; text-decoration:underline">`6.0`</span>
`shotgunspread2 `<span style="color:red; text-decoration:line-through">`2`</span><span style="color:green; text-decoration:underline">`3.0`</span>
<span style="color:green; text-decoration:underline">`shotgunspreadmax1 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunspreadmax2 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunspreadmin1 16.0`</span>
<span style="color:green; text-decoration:underline">`shotgunspreadmin2 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunspreadz1 1.0`</span>
<span style="color:green; text-decoration:underline">`shotgunspreadz2 4.0`</span>
<span style="color:green; text-decoration:underline">`shotgunstunfall1 0.0`</span>
<span style="color:green; text-decoration:underline">`shotgunstunfall2 0.0`</span>
`shotgunstunscale1 1.0`
`shotgunstunscale2 0.5`
`shotgunstuntime1 100`
`shotgunstuntime2 100`
`shotgunsub1 1`
`shotgunsub2 2`
<span style="color:green; text-decoration:underline">`shotguntaper1 0`</span>
<span style="color:green; text-decoration:underline">`shotguntaper2 0`</span>
`shotguntaperin1 0.0`
`shotguntaperin2 0.0`
`shotguntaperout1 0.0`
`shotguntaperout2 0.0`
<span style="color:green; text-decoration:underline">`shotgunteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`shotgunteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`shotgunteampenalty1 1.0`</span>
<span style="color:green; text-decoration:underline">`shotgunteampenalty2 1.0`</span>
`shotguntime2 5000`
<span style="color:red; text-decoration:line-through">`shotguntorsodmg1`</span><span style="color:green; text-decoration:underline">`shotguntorsodamage1`</span>` 0.6`
<span style="color:red; text-decoration:line-through">`shotguntorsodmg2 0.7`</span><span style="color:green; text-decoration:underline">`shotguntorsodamage2 0.6`</span>
`shotguntrace1 1.0`
`shotguntrace2 1.0`
<span style="color:green; text-decoration:underline">`shotgunvisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`shotgunvisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`shotgunvistime1 0`</span>
<span style="color:green; text-decoration:underline">`shotgunvistime2 0`</span>
`shotgunwaterfric1 2.0`
`shotgunwaterfric2 2.0`
<span style="color:green; text-decoration:underline">`shotgunwavepush1 1.5`</span>
<span style="color:green; text-decoration:underline">`shotgunwavepush2 1.5`</span>
`shotgunweight1 0.0`
`shotgunweight2 250.0`
<span style="color:red; text-decoration:line-through">`shotgunwhipdmg1`</span><span style="color:green; text-decoration:underline">`shotgunwhipdamage1`</span>` 0.8`
<span style="color:red; text-decoration:line-through">`shotgunwhipdmg2 0.9`</span>
<span style="color:red; text-decoration:line-through">`shotgunzdiv1 1`</span>
<span style="color:red; text-decoration:line-through">`shotgunzdiv2 4`</span><span style="color:green; text-decoration:underline">`shotgunwhipdamage2 0.8`</span>
`shotgunzooms 0`
<span style="color:red; text-decoration:line-through">`slidecoastforce -1.0`</span><span style="color:green; text-decoration:underline">`slidecoast 40.0`</span>
`slidecoastscale 1.0`
<span style="color:red; text-decoration:line-through">`smgadd 40`</span><span style="color:green; text-decoration:underline">`smallmapmax 6`</span>
<span style="color:red; text-decoration:line-through">`smgadelay1 100`</span><span style="color:green; text-decoration:underline">`smallmaps "bath bloodlust darkness deadsimple dutility echo error fourplex ghost longestyard livefire stone panic vault wet"`</span>
<span style="color:red; text-decoration:line-through">`smgadelay2 450`</span><span style="color:green; text-decoration:underline">`smgadd 50`</span>
`smgaidist1 512.0`
`smgaidist2 96.0`
`smgaiskew1 20`
`smgaiskew2 20`
<span style="color:red; text-decoration:line-through">`smgallowed 2`</span><span style="color:green; text-decoration:underline">`smgattackdelay1 100`</span>
<span style="color:green; text-decoration:underline">`smgattackdelay2 400`</span>
`smgcarried 1`
`smgcollide1 `<span style="color:red; text-decoration:line-through">`118`</span><span style="color:green; text-decoration:underline">`629`</span>
`smgcollide2 `<span style="color:red; text-decoration:line-through">`117`</span><span style="color:green; text-decoration:underline">`4157`</span>
`smgcolour `<span style="color:red; text-decoration:line-through">`0xFF6600`</span><span style="color:green; text-decoration:underline">`0xF05820`</span>
`smgcooked1 0`
`smgcooked2 0`
<span style="color:red; text-decoration:line-through">`smgcritdash1 0`</span>
<span style="color:red; text-decoration:line-through">`smgcritdash2 0`</span>
<span style="color:red; text-decoration:line-through">`smgcritdist 128.0`</span>
<span style="color:red; text-decoration:line-through">`smgcritmult 3.0`</span>
`smgdamage2 4`
`smgdelta1 10.0`
`smgdelta2 1000.0`
<span style="color:red; text-decoration:line-through">`smgedelay1 200`</span><span style="color:green; text-decoration:underline">`smgdrill1 2`</span>
<span style="color:red; text-decoration:line-through">`smgedelay2 200`</span><span style="color:green; text-decoration:underline">`smgdrill2 0`</span>
`smgelasticity1 0.65`
`smgelasticity2 0.45`
<span style="color:green; text-decoration:underline">`smgescapedelay1 200`</span>
<span style="color:green; text-decoration:underline">`smgescapedelay2 200`</span>
`smgexplcol2 `<span style="color:red; text-decoration:line-through">`0xFF6600`</span><span style="color:green; text-decoration:underline">`0xF05820`</span>
`smgexplode1 `<span style="color:red; text-decoration:line-through">`0`</span><span style="color:green; text-decoration:underline">`0.0`</span>
`smgexplode2 `<span style="color:red; text-decoration:line-through">`0`</span><span style="color:green; text-decoration:underline">`0.0`</span>
`smgextinguish1 2`
`smgextinguish2 2`
`smgflakcollide1 `<span style="color:red; text-decoration:line-through">`118`</span><span style="color:green; text-decoration:underline">`117`</span>
`smgflakcollide2 `<span style="color:red; text-decoration:line-through">`118`</span><span style="color:green; text-decoration:underline">`117`</span>
<span style="color:red; text-decoration:line-through">`smgflakdmg1 16`</span><span style="color:green; text-decoration:underline">`smgflakdamage1 18`</span>
<span style="color:red; text-decoration:line-through">`smgflakdmg2 4`</span><span style="color:green; text-decoration:underline">`smgflakdamage2 10`</span>
<span style="color:green; text-decoration:underline">`smgflakdelta1 10.0`</span>
<span style="color:green; text-decoration:underline">`smgflakdelta2 1000.0`</span>
<span style="color:green; text-decoration:underline">`smgflakdrill1 2`</span>
<span style="color:green; text-decoration:underline">`smgflakdrill2 0`</span>
<span style="color:green; text-decoration:underline">`smgflakelasticity1 0.65`</span>
<span style="color:green; text-decoration:underline">`smgflakelasticity2 0.45`</span>
<span style="color:green; text-decoration:underline">`smgflakexplcol1 0xF05820`</span>
<span style="color:red; text-decoration:line-through">`smgflakffwd1`</span><span style="color:green; text-decoration:underline">`smgflakexplcol2 0xF05820`</span>
<span style="color:green; text-decoration:underline">`smgflakexplode1`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`smgflakffwd2`</span><span style="color:green; text-decoration:underline">`smgflakexplode2`</span>` 0.0`
<span style="color:green; text-decoration:underline">`smgflakextinguish1 2`</span>
<span style="color:green; text-decoration:underline">`smgflakextinguish2 2`</span>
<span style="color:green; text-decoration:underline">`smgflakguided1 0`</span>
<span style="color:green; text-decoration:underline">`smgflakguided2 0`</span>
<span style="color:green; text-decoration:underline">`smgflakguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`smgflakguideddelay2 100`</span>
<span style="color:green; text-decoration:underline">`smgflakheadmin1 0.0`</span>
<span style="color:green; text-decoration:underline">`smgflakheadmin2 0.0`</span>
<span style="color:green; text-decoration:underline">`smgflakhitpush1 50.0`</span>
<span style="color:green; text-decoration:underline">`smgflakhitpush2 50.0`</span>
<span style="color:green; text-decoration:underline">`smgflakinteracts1 1`</span>
<span style="color:green; text-decoration:underline">`smgflakinteracts2 3`</span>
<span style="color:green; text-decoration:underline">`smgflaklegdamage1 0.3`</span>
<span style="color:green; text-decoration:underline">`smgflaklegdamage2 0.3`</span>
`smgflakminspeed2 `<span style="color:red; text-decoration:line-through">`25.0`</span><span style="color:green; text-decoration:underline">`50.0`</span>
<span style="color:red; text-decoration:line-through">`smgflakoffset1 8.0`</span><span style="color:green; text-decoration:underline">`smgflakpartcol1 0xF05820`</span>
<span style="color:red; text-decoration:line-through">`smgflakoffset2 8.0`</span><span style="color:green; text-decoration:underline">`smgflakpartcol2 0xF05820`</span>
<span style="color:red; text-decoration:line-through">`smgflakrays1 5`</span><span style="color:green; text-decoration:underline">`smgflakpartlen1 7.5`</span>
<span style="color:green; text-decoration:underline">`smgflakpartlen2 7.5`</span>
<span style="color:green; text-decoration:underline">`smgflakpartsize1 0.35`</span>
<span style="color:green; text-decoration:underline">`smgflakpartsize2 0.35`</span>
<span style="color:red; text-decoration:line-through">`smgflakrays2 35`</span><span style="color:green; text-decoration:underline">`smgflakparttype1 4`</span>
<span style="color:green; text-decoration:underline">`smgflakparttype2 4`</span>
<span style="color:green; text-decoration:underline">`smgflakproxdelay1 0`</span>
<span style="color:green; text-decoration:underline">`smgflakproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`smgflakproxdist1 0.0`</span>
<span style="color:green; text-decoration:underline">`smgflakproxdist2 0.0`</span>
<span style="color:green; text-decoration:underline">`smgflakproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`smgflakproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`smgflakproxtype1 0`</span>
<span style="color:red; text-decoration:line-through">`smgflakrel1`</span><span style="color:green; text-decoration:underline">`smgflakproxtype2 0`</span>
<span style="color:green; text-decoration:underline">`smgflakradial1 0`</span>
<span style="color:green; text-decoration:underline">`smgflakradial2 0`</span>
<span style="color:green; text-decoration:underline">`smgflakradius1 1.0`</span>
<span style="color:green; text-decoration:underline">`smgflakradius2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`smgflakrel2 0.05`</span><span style="color:green; text-decoration:underline">`smgflakreflectivity1 0.0`</span>
<span style="color:green; text-decoration:underline">`smgflakreflectivity2 0.0`</span>
<span style="color:green; text-decoration:underline">`smgflakresidual1 0`</span>
<span style="color:green; text-decoration:underline">`smgflakresidual2 0`</span>
<span style="color:green; text-decoration:underline">`smgflakselfdamage1 0.5`</span>
<span style="color:red; text-decoration:line-through">`smgflakscale1`</span><span style="color:green; text-decoration:underline">`smgflakselfdamage2 0.5`</span>
<span style="color:green; text-decoration:underline">`smgflakstunfall1 0.0`</span>
<span style="color:green; text-decoration:underline">`smgflakstunfall2 0.0`</span>
<span style="color:green; text-decoration:underline">`smgflakstunscale1 0.5`</span>
<span style="color:green; text-decoration:underline">`smgflakstunscale2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`smgflakscale2`</span><span style="color:green; text-decoration:underline">`smgflakstuntime1 100`</span>
<span style="color:green; text-decoration:underline">`smgflakstuntime2 200`</span>
<span style="color:green; text-decoration:underline">`smgflaktaper1 0`</span>
<span style="color:green; text-decoration:underline">`smgflaktaper2 0`</span>
<span style="color:green; text-decoration:underline">`smgflaktaperin1 0.0`</span>
<span style="color:green; text-decoration:underline">`smgflaktaperin2 0.0`</span>
<span style="color:green; text-decoration:underline">`smgflaktaperout1 0.0`</span>
<span style="color:green; text-decoration:underline">`smgflaktaperout2 0.0`</span>
<span style="color:green; text-decoration:underline">`smgflakteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`smgflakteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`smgflakteampenalty1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`smgflakskew1`</span><span style="color:green; text-decoration:underline">`smgflakteampenalty2 0.0`</span>
<span style="color:green; text-decoration:underline">`smgflaktorsodamage1 0.6`</span>
<span style="color:green; text-decoration:underline">`smgflaktorsodamage2 0.6`</span>
<span style="color:green; text-decoration:underline">`smgflakvisfade1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`smgflakskew2`</span><span style="color:green; text-decoration:underline">`smgflakvisfade2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`smgflakspeed1`</span><span style="color:green; text-decoration:underline">`smgflakvistime1`</span>` 0`
<span style="color:red; text-decoration:line-through">`smgflakspeed2`</span><span style="color:green; text-decoration:underline">`smgflakvistime2`</span>` 0`
<span style="color:red; text-decoration:line-through">`smgflakspread1 0.2`</span><span style="color:green; text-decoration:underline">`smgflakwaterfric1 2.0`</span>
<span style="color:red; text-decoration:line-through">`smgflakspread2`</span><span style="color:green; text-decoration:underline">`smgflakwaterfric2 2.0`</span>
<span style="color:green; text-decoration:underline">`smgflakwavepush1 1.5`</span>
<span style="color:green; text-decoration:underline">`smgflakwavepush2 1.5`</span>
<span style="color:green; text-decoration:underline">`smgflakweight1 0.0`</span>
<span style="color:green; text-decoration:underline">`smgflakweight2 0.0`</span>
<span style="color:green; text-decoration:underline">`smgflakwhipdamage1 0.8`</span>
<span style="color:green; text-decoration:underline">`smgflakwhipdamage2 0.8`</span>
<span style="color:green; text-decoration:underline">`smgfragdelay1 0`</span>
<span style="color:green; text-decoration:underline">`smgfragdelay2 3`</span>
<span style="color:green; text-decoration:underline">`smgfragjump1 0.0`</span>
<span style="color:green; text-decoration:underline">`smgfragjump2 0.0`</span>
<span style="color:green; text-decoration:underline">`smgfragoffset1 4.0`</span>
<span style="color:green; text-decoration:underline">`smgfragoffset2 4.0`</span>
<span style="color:green; text-decoration:underline">`smgfragrays1 5`</span>
<span style="color:green; text-decoration:underline">`smgfragrays2 20`</span>
<span style="color:green; text-decoration:underline">`smgfragrel1 1.0`</span>
<span style="color:green; text-decoration:underline">`smgfragrel2 0.1`</span>
<span style="color:green; text-decoration:underline">`smgfragscale1 1.0`</span>
<span style="color:green; text-decoration:underline">`smgfragscale2 1.0`</span>
<span style="color:green; text-decoration:underline">`smgfragskew1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`smgflaktime1`</span><span style="color:green; text-decoration:underline">`smgfragskew2 1.0`</span>
<span style="color:green; text-decoration:underline">`smgfragspeed1 0`</span>
<span style="color:green; text-decoration:underline">`smgfragspeed2 250`</span>
<span style="color:green; text-decoration:underline">`smgfragspread1 0.2`</span>
<span style="color:green; text-decoration:underline">`smgfragspread2 0.5`</span>
<span style="color:green; text-decoration:underline">`smgfragtime1`</span>` 500`
<span style="color:red; text-decoration:line-through">`smgflaktime2 800`</span><span style="color:green; text-decoration:underline">`smgfragtime2 1000`</span>
<span style="color:red; text-decoration:line-through">`smgflakweap1`</span><span style="color:green; text-decoration:underline">`smgfragweap1`</span>` -1`
<span style="color:red; text-decoration:line-through">`smgflakweap2 14`</span><span style="color:green; text-decoration:underline">`smgfragweap2 15`</span>
`smgfrequency 1.0`
`smgfullauto1 1`
`smgfullauto2 1`
<span style="color:red; text-decoration:line-through">`smggdelay1 0`</span>
<span style="color:red; text-decoration:line-through">`smggdelay2 100`</span>
`smgguided1 0`
`smgguided2 0`
<span style="color:green; text-decoration:underline">`smgguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`smgguideddelay2 100`</span>
`smgheadmin1 0.0`
`smgheadmin2 0.0`
`smghitpush1 50.0`
`smghitpush2 50.0`
<span style="color:red; text-decoration:line-through">`smgjamchance 25`</span><span style="color:green; text-decoration:underline">`smginteracts1 1`</span>
<span style="color:green; text-decoration:underline">`smginteracts2 3`</span>
`smgkickpush1 5.0`
`smgkickpush2 10.0`
`smglaser 0`
<span style="color:red; text-decoration:line-through">`smglegsdmg1 0.35`</span><span style="color:green; text-decoration:underline">`smglegdamage1 0.3`</span>
<span style="color:red; text-decoration:line-through">`smglegsdmg2 0.35`</span><span style="color:green; text-decoration:underline">`smglegdamage2 0.3`</span>
`smglimspeed1 0`
`smglimspeed2 0`
`smgmax `<span style="color:red; text-decoration:line-through">`40`</span>
<span style="color:red; text-decoration:line-through">`smgmaxspread1 0`</span>
<span style="color:red; text-decoration:line-through">`smgmaxspread2 0`</span><span style="color:green; text-decoration:underline">`50`</span>
`smgminspeed1 25.0`
`smgminspeed2 25.0`
<span style="color:red; text-decoration:line-through">`smgminspread1 0`</span><span style="color:green; text-decoration:underline">`smgmodes -64`</span>
<span style="color:red; text-decoration:line-through">`smgminspread2 0`</span><span style="color:green; text-decoration:underline">`smgmuts -56`</span>
`smgname "smg"`
`smgpartcol1 `<span style="color:red; text-decoration:line-through">`0xFF6600`</span><span style="color:green; text-decoration:underline">`0xF05820`</span>
`smgpartcol2 `<span style="color:red; text-decoration:line-through">`0xFF6600`</span><span style="color:green; text-decoration:underline">`0xF05820`</span>
`smgpartlen1 `<span style="color:red; text-decoration:line-through">`35.0`</span><span style="color:green; text-decoration:underline">`30.0`</span>
`smgpartlen2 `<span style="color:red; text-decoration:line-through">`20.0`</span><span style="color:green; text-decoration:underline">`15.0`</span>
`smgpartsize1 0.5`
`smgpartsize2 0.35`
`smgparttype1 4`
`smgparttype2 4`
<span style="color:red; text-decoration:line-through">`smgpdelay1 0`</span>
<span style="color:red; text-decoration:line-through">`smgpdelay2 0`</span>
`smgpower1 0`
`smgpower2 0`
<span style="color:red; text-decoration:line-through">`smgpusharea 1.5`</span><span style="color:green; text-decoration:underline">`smgprojdelay1 0`</span>
<span style="color:green; text-decoration:underline">`smgprojdelay2 0`</span>
<span style="color:green; text-decoration:underline">`smgproxdelay1 0`</span>
<span style="color:green; text-decoration:underline">`smgproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`smgproxdist1 0.0`</span>
<span style="color:green; text-decoration:underline">`smgproxdist2 0.0`</span>
<span style="color:green; text-decoration:underline">`smgproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`smgproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`smgproxtype1 0`</span>
<span style="color:green; text-decoration:underline">`smgproxtype2 0`</span>
`smgradial1 0`
`smgradial2 0`
`smgradius1 1.0`
`smgradius2 1.0`
`smgrays1 1`
`smgrays2 1`
<span style="color:red; text-decoration:line-through">`smgrdelay 1500`</span>
`smgreflectivity1 0.0`
`smgreflectivity2 0.0`
`smgrelativity1 0.05`
`smgrelativity2 0.05`
<span style="color:green; text-decoration:underline">`smgreloaddelay 2000`</span>
`smgreloads -1`
`smgresidual1 0`
`smgresidual2 0`
<span style="color:red; text-decoration:line-through">`smgselfdmg1`</span><span style="color:green; text-decoration:underline">`smgselfdamage1`</span>` 0.5`
<span style="color:red; text-decoration:line-through">`smgselfdmg2`</span><span style="color:green; text-decoration:underline">`smgselfdamage2`</span>` 0.5 `<span style="color:red; text-decoration:line-through">`smgslow1 0.0`</span>
<span style="color:red; text-decoration:line-through">`smgslow2 0.0`</span>
`smgspeed1 2500`
`smgspeed2 `<span style="color:red; text-decoration:line-through">`450`</span><span style="color:green; text-decoration:underline">`500`</span>
`smgspread1 `<span style="color:red; text-decoration:line-through">`3`</span><span style="color:green; text-decoration:underline">`3.0`</span>
`smgspread2 `<span style="color:red; text-decoration:line-through">`6`</span><span style="color:green; text-decoration:underline">`3.0`</span>
<span style="color:red; text-decoration:line-through">`smgstunscale1`</span><span style="color:green; text-decoration:underline">`smgspreadmax1 0.0`</span>
<span style="color:green; text-decoration:underline">`smgspreadmax2 0.0`</span>
<span style="color:green; text-decoration:underline">`smgspreadmin1 0.0`</span>
<span style="color:green; text-decoration:underline">`smgspreadmin2 0.0`</span>
<span style="color:green; text-decoration:underline">`smgspreadz1 1.0`</span>
<span style="color:green; text-decoration:underline">`smgspreadz2`</span>` 2.0`
<span style="color:green; text-decoration:underline">`smgstunfall1 0.0`</span>
<span style="color:green; text-decoration:underline">`smgstunfall2 0.0`</span>
<span style="color:green; text-decoration:underline">`smgstunscale1 0.5`</span>
`smgstuntime1 `<span style="color:red; text-decoration:line-through">`200`</span><span style="color:green; text-decoration:underline">`100`</span>
`smgstuntime2 200`
`smgsub1 1`
`smgsub2 `<span style="color:red; text-decoration:line-through">`4`</span><span style="color:green; text-decoration:underline">`5`</span>
<span style="color:green; text-decoration:underline">`smgtaper1 0`</span>
<span style="color:green; text-decoration:underline">`smgtaper2 0`</span>
`smgtaperin1 0.0`
`smgtaperin2 0.0`
`smgtaperout1 0.0`
`smgtaperout2 0.0`
<span style="color:green; text-decoration:underline">`smgteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`smgteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`smgteampenalty1 1.0`</span>
<span style="color:green; text-decoration:underline">`smgteampenalty2 1.0`</span>
`smgtime2 `<span style="color:red; text-decoration:line-through">`500`</span><span style="color:green; text-decoration:underline">`2000`</span>
<span style="color:red; text-decoration:line-through">`smgtorsodmg1 0.7`</span><span style="color:green; text-decoration:underline">`smgtorsodamage1 0.6`</span>
<span style="color:red; text-decoration:line-through">`smgtorsodmg2 0.7`</span><span style="color:green; text-decoration:underline">`smgtorsodamage2 0.6`</span>
`smgtrace1 1.0`
`smgtrace2 1.0`
<span style="color:green; text-decoration:underline">`smgvisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`smgvisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`smgvistime1 0`</span>
<span style="color:green; text-decoration:underline">`smgvistime2 0`</span>
`smgwaterfric1 2.0`
`smgwaterfric2 2.0`
<span style="color:green; text-decoration:underline">`smgwavepush1 1.5`</span>
<span style="color:green; text-decoration:underline">`smgwavepush2 1.5`</span>
`smgweight1 0.0`
`smgweight2 0.0`
<span style="color:red; text-decoration:line-through">`smgwhipdmg1`</span><span style="color:green; text-decoration:underline">`smgwhipdamage1`</span>` 0.8`
<span style="color:red; text-decoration:line-through">`smgwhipdmg2`</span><span style="color:green; text-decoration:underline">`smgwhipdamage2`</span>` 0.8 `<span style="color:red; text-decoration:line-through">`smgzdiv1 2`</span>
<span style="color:red; text-decoration:line-through">`smgzdiv2 2`</span>
`smgzooms 0`
<span style="color:green; text-decoration:underline">`spawnarmour 0`</span>
`spawndelay 5000`
`spawngrenades 0`
`spawnhealth 100`
<span style="color:green; text-decoration:underline">`spawnmines 0`</span>
`spawnprotect 3000`
`spawnrotate 2`
`spawnweapon 1`
<span style="color:red; text-decoration:line-through">`spreebonus`</span><span style="color:green; text-decoration:underline">`speclock 3`</span>
<span style="color:green; text-decoration:underline">`spreebreaker`</span>` 1`
`spreecount 5`
`spreepoints 1`
`stillspread 0.0`
<span style="color:green; text-decoration:underline">`stunlimited 0.75`</span>
<span style="color:green; text-decoration:underline">`stunscale 1.0`</span>
`swordadd 1`
<span style="color:red; text-decoration:line-through">`swordadelay1 500`</span>
<span style="color:red; text-decoration:line-through">`swordadelay2 750`</span>
`swordaidist1 48.0`
`swordaidist2 48.0`
`swordaiskew1 1`
`swordaiskew2 1`
<span style="color:red; text-decoration:line-through">`swordallowed 2`</span><span style="color:green; text-decoration:underline">`swordattackdelay1 600`</span>
<span style="color:green; text-decoration:underline">`swordattackdelay2 1000`</span>
`swordcarried 1`
`swordcollide1 `<span style="color:red; text-decoration:line-through">`182`</span><span style="color:green; text-decoration:underline">`1137`</span>
`swordcollide2 `<span style="color:red; text-decoration:line-through">`182`</span><span style="color:green; text-decoration:underline">`1137`</span>
`swordcolour `<span style="color:red; text-decoration:line-through">`0x4444FF`</span><span style="color:green; text-decoration:underline">`0x4040F0`</span>
`swordcooked1 0`
`swordcooked2 0`
<span style="color:red; text-decoration:line-through">`swordcritdash1 500`</span>
<span style="color:red; text-decoration:line-through">`swordcritdash2 500`</span>
<span style="color:red; text-decoration:line-through">`swordcritdist 0.0`</span>
<span style="color:red; text-decoration:line-through">`swordcritmult 2.0`</span>
`sworddamage2 `<span style="color:red; text-decoration:line-through">`60`</span><span style="color:green; text-decoration:underline">`50`</span>
`sworddelta1 10.0`
`sworddelta2 10.0`
<span style="color:red; text-decoration:line-through">`swordedelay1 200`</span><span style="color:green; text-decoration:underline">`sworddrill1 0`</span>
<span style="color:red; text-decoration:line-through">`swordedelay2 200`</span><span style="color:green; text-decoration:underline">`sworddrill2 0`</span>
`swordelasticity1 0.5`
`swordelasticity2 0.5`
<span style="color:green; text-decoration:underline">`swordescapedelay1 200`</span>
<span style="color:green; text-decoration:underline">`swordescapedelay2 200`</span>
`swordexplcol2 `<span style="color:red; text-decoration:line-through">`0x4444FF`</span><span style="color:green; text-decoration:underline">`0x4040F0`</span>
`swordexplode1 `<span style="color:red; text-decoration:line-through">`0`</span><span style="color:green; text-decoration:underline">`0.0`</span>
`swordexplode2 `<span style="color:red; text-decoration:line-through">`0`</span><span style="color:green; text-decoration:underline">`0.0`</span>
`swordextinguish1 2`
`swordextinguish2 2`
`swordflakcollide1 `<span style="color:red; text-decoration:line-through">`182`</span><span style="color:green; text-decoration:underline">`1141`</span>
`swordflakcollide2 `<span style="color:red; text-decoration:line-through">`182`</span><span style="color:green; text-decoration:underline">`1141`</span>
<span style="color:red; text-decoration:line-through">`swordflakdmg1 15`</span><span style="color:green; text-decoration:underline">`swordflakdamage1 25`</span>
<span style="color:red; text-decoration:line-through">`swordflakdmg2 30`</span><span style="color:green; text-decoration:underline">`swordflakdamage2 50`</span>
<span style="color:red; text-decoration:line-through">`swordflakffwd1`</span><span style="color:green; text-decoration:underline">`swordflakdelta1 10.0`</span>
<span style="color:green; text-decoration:underline">`swordflakdelta2 10.0`</span>
<span style="color:green; text-decoration:underline">`swordflakdrill1 0`</span>
<span style="color:green; text-decoration:underline">`swordflakdrill2 0`</span>
<span style="color:green; text-decoration:underline">`swordflakelasticity1 0.5`</span>
<span style="color:green; text-decoration:underline">`swordflakelasticity2 0.5`</span>
<span style="color:green; text-decoration:underline">`swordflakexplcol1 0x4040F0`</span>
<span style="color:green; text-decoration:underline">`swordflakexplcol2 0x4040F0`</span>
<span style="color:green; text-decoration:underline">`swordflakexplode1`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`swordflakffwd2`</span><span style="color:green; text-decoration:underline">`swordflakexplode2`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`swordflakminspeed1`</span><span style="color:green; text-decoration:underline">`swordflakextinguish1 2`</span>
<span style="color:green; text-decoration:underline">`swordflakextinguish2 2`</span>
<span style="color:green; text-decoration:underline">`swordflakguided1 0`</span>
<span style="color:green; text-decoration:underline">`swordflakguided2 0`</span>
<span style="color:green; text-decoration:underline">`swordflakguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`swordflakguideddelay2 0`</span>
<span style="color:green; text-decoration:underline">`swordflakheadmin1`</span>` 0.0`
<span style="color:green; text-decoration:underline">`swordflakheadmin2 0.0`</span>
<span style="color:green; text-decoration:underline">`swordflakhitpush1 50.0`</span>
<span style="color:green; text-decoration:underline">`swordflakhitpush2 100.0`</span>
<span style="color:green; text-decoration:underline">`swordflakinteracts1 0`</span>
<span style="color:green; text-decoration:underline">`swordflakinteracts2 0`</span>
<span style="color:green; text-decoration:underline">`swordflaklegdamage1 0.3`</span>
<span style="color:green; text-decoration:underline">`swordflaklegdamage2 0.3`</span>
<span style="color:green; text-decoration:underline">`swordflakminspeed1 50.0`</span>
<span style="color:green; text-decoration:underline">`swordflakpartcol1 0x4040F0`</span>
<span style="color:green; text-decoration:underline">`swordflakpartcol2 0x4040F0`</span>
<span style="color:green; text-decoration:underline">`swordflakpartlen1 0.0`</span>
<span style="color:green; text-decoration:underline">`swordflakpartlen2 0.0`</span>
<span style="color:green; text-decoration:underline">`swordflakpartsize1 1.0`</span>
<span style="color:green; text-decoration:underline">`swordflakpartsize2 1.25`</span>
<span style="color:green; text-decoration:underline">`swordflakparttype1 2`</span>
<span style="color:green; text-decoration:underline">`swordflakparttype2 2`</span>
<span style="color:green; text-decoration:underline">`swordflakproxdelay1 0`</span>
<span style="color:green; text-decoration:underline">`swordflakproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`swordflakproxdist1 0.0`</span>
<span style="color:green; text-decoration:underline">`swordflakproxdist2 0.0`</span>
<span style="color:green; text-decoration:underline">`swordflakproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`swordflakproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`swordflakproxtype1 0`</span>
<span style="color:green; text-decoration:underline">`swordflakproxtype2 0`</span>
<span style="color:green; text-decoration:underline">`swordflakradial1 0`</span>
<span style="color:green; text-decoration:underline">`swordflakradial2 0`</span>
<span style="color:green; text-decoration:underline">`swordflakradius1 1.0`</span>
<span style="color:green; text-decoration:underline">`swordflakradius2 1.0`</span>
<span style="color:green; text-decoration:underline">`swordflakreflectivity1 0.0`</span>
<span style="color:green; text-decoration:underline">`swordflakreflectivity2 0.0`</span>
<span style="color:green; text-decoration:underline">`swordflakresidual1 2`</span>
<span style="color:green; text-decoration:underline">`swordflakresidual2 2`</span>
<span style="color:green; text-decoration:underline">`swordflakselfdamage1 0.0`</span>
<span style="color:green; text-decoration:underline">`swordflakselfdamage2 0.0`</span>
<span style="color:green; text-decoration:underline">`swordflakstunfall1 0.0`</span>
<span style="color:green; text-decoration:underline">`swordflakstunfall2 0.0`</span>
<span style="color:green; text-decoration:underline">`swordflakstunscale1 1.0`</span>
<span style="color:green; text-decoration:underline">`swordflakstunscale2 2.0`</span>
<span style="color:green; text-decoration:underline">`swordflakstuntime1 200`</span>
<span style="color:green; text-decoration:underline">`swordflakstuntime2 200`</span>
<span style="color:green; text-decoration:underline">`swordflaktaper1 0`</span>
<span style="color:green; text-decoration:underline">`swordflaktaper2 0`</span>
<span style="color:green; text-decoration:underline">`swordflaktaperin1 0.0`</span>
<span style="color:green; text-decoration:underline">`swordflaktaperin2 0.0`</span>
<span style="color:green; text-decoration:underline">`swordflaktaperout1 0.0`</span>
<span style="color:green; text-decoration:underline">`swordflaktaperout2 0.0`</span>
<span style="color:green; text-decoration:underline">`swordflakteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`swordflakteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`swordflakteampenalty1 1.0`</span>
<span style="color:green; text-decoration:underline">`swordflakteampenalty2 1.0`</span>
<span style="color:green; text-decoration:underline">`swordflaktorsodamage1 0.65`</span>
<span style="color:green; text-decoration:underline">`swordflaktorsodamage2 0.65`</span>
<span style="color:green; text-decoration:underline">`swordflakvisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`swordflakvisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`swordflakvistime1 0`</span>
<span style="color:green; text-decoration:underline">`swordflakvistime2 0`</span>
<span style="color:green; text-decoration:underline">`swordflakwaterfric1 0.0`</span>
<span style="color:green; text-decoration:underline">`swordflakwaterfric2 0.0`</span>
<span style="color:green; text-decoration:underline">`swordflakwavepush1 1.5`</span>
<span style="color:green; text-decoration:underline">`swordflakwavepush2 1.5`</span>
<span style="color:green; text-decoration:underline">`swordflakweight1 0.0`</span>
<span style="color:green; text-decoration:underline">`swordflakweight2 0.0`</span>
<span style="color:green; text-decoration:underline">`swordflakwhipdamage1 0.8`</span>
<span style="color:green; text-decoration:underline">`swordflakwhipdamage2 0.8`</span>
<span style="color:green; text-decoration:underline">`swordfragdelay1 0`</span>
<span style="color:green; text-decoration:underline">`swordfragdelay2 0`</span>
<span style="color:green; text-decoration:underline">`swordfragjump1 0.0`</span>
<span style="color:green; text-decoration:underline">`swordfragjump2`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`swordflakoffset1 8.0`</span><span style="color:green; text-decoration:underline">`swordfragoffset1 4.0`</span>
<span style="color:red; text-decoration:line-through">`swordflakoffset2 8.0`</span><span style="color:green; text-decoration:underline">`swordfragoffset2 4.0`</span>
<span style="color:red; text-decoration:line-through">`swordflakrays1`</span><span style="color:green; text-decoration:underline">`swordfragrays1`</span>` 5`
<span style="color:red; text-decoration:line-through">`swordflakrays2`</span><span style="color:green; text-decoration:underline">`swordfragrays2`</span>` 5`
<span style="color:red; text-decoration:line-through">`swordflakrel1`</span><span style="color:green; text-decoration:underline">`swordfragrel1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`swordflakrel2`</span><span style="color:green; text-decoration:underline">`swordfragrel2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`swordflakscale1`</span><span style="color:green; text-decoration:underline">`swordfragscale1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`swordflakscale2`</span><span style="color:green; text-decoration:underline">`swordfragscale2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`swordflakskew1`</span><span style="color:green; text-decoration:underline">`swordfragskew1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`swordflakskew2`</span><span style="color:green; text-decoration:underline">`swordfragskew2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`swordflakspeed1`</span><span style="color:green; text-decoration:underline">`swordfragspeed1`</span>` 0`
<span style="color:red; text-decoration:line-through">`swordflakspeed2`</span><span style="color:green; text-decoration:underline">`swordfragspeed2`</span>` 0`
<span style="color:red; text-decoration:line-through">`swordflakspread1`</span><span style="color:green; text-decoration:underline">`swordfragspread1`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`swordflakspread2`</span><span style="color:green; text-decoration:underline">`swordfragspread2`</span>` 1.0`
<span style="color:red; text-decoration:line-through">`swordflaktime1`</span><span style="color:green; text-decoration:underline">`swordfragtime1`</span>` 500`
<span style="color:red; text-decoration:line-through">`swordflaktime2`</span><span style="color:green; text-decoration:underline">`swordfragtime2`</span>` 500`
<span style="color:red; text-decoration:line-through">`swordflakweap1`</span><span style="color:green; text-decoration:underline">`swordfragweap1`</span>` -1`
<span style="color:red; text-decoration:line-through">`swordflakweap2`</span><span style="color:green; text-decoration:underline">`swordfragweap2`</span>` -1`
`swordfrequency 1.0`
`swordfullauto1 1`
`swordfullauto2 1`
<span style="color:red; text-decoration:line-through">`swordgdelay1 0`</span>
<span style="color:red; text-decoration:line-through">`swordgdelay2 0`</span>
`swordguided1 0`
`swordguided2 0`
<span style="color:green; text-decoration:underline">`swordguideddelay1 0`</span>
<span style="color:green; text-decoration:underline">`swordguideddelay2 0`</span>
`swordheadmin1 0.0`
`swordheadmin2 0.0`
`swordhitpush1 50.0`
`swordhitpush2 100.0`
<span style="color:red; text-decoration:line-through">`swordjamchance`</span><span style="color:green; text-decoration:underline">`swordinteracts1 0`</span>
<span style="color:green; text-decoration:underline">`swordinteracts2`</span>` 0`
`swordkickpush1 0.0`
`swordkickpush2 0.0`
`swordlaser 0`
<span style="color:red; text-decoration:line-through">`swordlegsdmg1`</span><span style="color:green; text-decoration:underline">`swordlegdamage1`</span>` 0.3`
<span style="color:red; text-decoration:line-through">`swordlegsdmg2`</span><span style="color:green; text-decoration:underline">`swordlegdamage2`</span>` 0.3`
`swordlimspeed1 0`
`swordlimspeed2 0`
`swordmax 1`
<span style="color:red; text-decoration:line-through">`swordmaxspread1 0`</span>
<span style="color:red; text-decoration:line-through">`swordmaxspread2 0`</span>
`swordminspeed1 0.0`
`swordminspeed2 0.0`
<span style="color:red; text-decoration:line-through">`swordminspread1 0`</span><span style="color:green; text-decoration:underline">`swordmodes -64`</span>
<span style="color:red; text-decoration:line-through">`swordminspread2 0`</span><span style="color:green; text-decoration:underline">`swordmuts -56`</span>
`swordname "sword"`
`swordpartcol1 `<span style="color:red; text-decoration:line-through">`0x4444FF`</span><span style="color:green; text-decoration:underline">`0x4040F0`</span>
`swordpartcol2 `<span style="color:red; text-decoration:line-through">`0x4444FF`</span><span style="color:green; text-decoration:underline">`0x4040F0`</span>
`swordpartlen1 0.0`
`swordpartlen2 0.0`
`swordpartsize1 1.0`
`swordpartsize2 1.25`
`swordparttype1 2`
`swordparttype2 2`
<span style="color:red; text-decoration:line-through">`swordpdelay1 10`</span>
<span style="color:red; text-decoration:line-through">`swordpdelay2 10`</span>
`swordpower1 0`
`swordpower2 0`
<span style="color:red; text-decoration:line-through">`swordpusharea 1.0`</span><span style="color:green; text-decoration:underline">`swordprojdelay1 10`</span>
<span style="color:green; text-decoration:underline">`swordprojdelay2 10`</span>
<span style="color:green; text-decoration:underline">`swordproxdelay1 0`</span>
<span style="color:green; text-decoration:underline">`swordproxdelay2 0`</span>
<span style="color:green; text-decoration:underline">`swordproxdist1 0.0`</span>
<span style="color:green; text-decoration:underline">`swordproxdist2 0.0`</span>
<span style="color:green; text-decoration:underline">`swordproxtime1 0`</span>
<span style="color:green; text-decoration:underline">`swordproxtime2 0`</span>
<span style="color:green; text-decoration:underline">`swordproxtype1 0`</span>
<span style="color:green; text-decoration:underline">`swordproxtype2 0`</span>
`swordradial1 0`
`swordradial2 0`
`swordradius1 1.0`
`swordradius2 1.0`
`swordrays1 1`
`swordrays2 1`
<span style="color:red; text-decoration:line-through">`swordrdelay 50`</span>
`swordreflectivity1 0.0`
`swordreflectivity2 0.0`
`swordrelativity1 0.0`
`swordrelativity2 0.0`
<span style="color:green; text-decoration:underline">`swordreloaddelay 50`</span>
`swordresidual1 2`
`swordresidual2 2`
<span style="color:red; text-decoration:line-through">`swordselfdmg1`</span><span style="color:green; text-decoration:underline">`swordselfdamage1`</span>` 0.0`
<span style="color:red; text-decoration:line-through">`swordselfdmg2 0.0`</span>
<span style="color:red; text-decoration:line-through">`swordslow1 0.0`</span>
<span style="color:red; text-decoration:line-through">`swordslow2`</span><span style="color:green; text-decoration:underline">`swordselfdamage2`</span>` 0.0`
`swordspeed1 0`
`swordspeed2 0`
`swordspread1 `<span style="color:red; text-decoration:line-through">`1`</span><span style="color:green; text-decoration:underline">`1.0`</span>
`swordspread2 `<span style="color:red; text-decoration:line-through">`1`</span><span style="color:green; text-decoration:underline">`1.0`</span>
<span style="color:green; text-decoration:underline">`swordspreadmax1 0.0`</span>
<span style="color:green; text-decoration:underline">`swordspreadmax2 0.0`</span>
<span style="color:green; text-decoration:underline">`swordspreadmin1 0.0`</span>
<span style="color:green; text-decoration:underline">`swordspreadmin2 0.0`</span>
<span style="color:green; text-decoration:underline">`swordspreadz1 1.0`</span>
<span style="color:green; text-decoration:underline">`swordspreadz2 1.0`</span>
<span style="color:green; text-decoration:underline">`swordstunfall1 0.0`</span>
<span style="color:green; text-decoration:underline">`swordstunfall2 0.0`</span>
`swordstunscale1 1.0`
`swordstunscale2 2.0`
`swordstuntime1 200`
`swordstuntime2 200`
`swordsub1 0`
`swordsub2 0`
<span style="color:green; text-decoration:underline">`swordtaper1 0`</span>
<span style="color:green; text-decoration:underline">`swordtaper2 0`</span>
`swordtaperin1 0.0`
`swordtaperin2 0.0`
`swordtaperout1 0.0`
`swordtaperout2 0.0`
<span style="color:green; text-decoration:underline">`swordteamdamage1 1.0`</span>
<span style="color:green; text-decoration:underline">`swordteamdamage2 1.0`</span>
<span style="color:green; text-decoration:underline">`swordteampenalty1 1.0`</span>
<span style="color:green; text-decoration:underline">`swordteampenalty2 1.0`</span>
`swordtime1 350`
`swordtime2 500`
<span style="color:red; text-decoration:line-through">`swordtorsodmg1`</span><span style="color:green; text-decoration:underline">`swordtorsodamage1`</span>` 0.65`
<span style="color:red; text-decoration:line-through">`swordtorsodmg2`</span><span style="color:green; text-decoration:underline">`swordtorsodamage2`</span>` 0.65`
`swordtrace1 `<span style="color:red; text-decoration:line-through">`3.0`</span><span style="color:green; text-decoration:underline">`2.0`</span>
`swordtrace2 `<span style="color:red; text-decoration:line-through">`5.0`</span><span style="color:green; text-decoration:underline">`2.0`</span>
<span style="color:green; text-decoration:underline">`swordvisfade1 1.0`</span>
<span style="color:green; text-decoration:underline">`swordvisfade2 1.0`</span>
<span style="color:green; text-decoration:underline">`swordvistime1 0`</span>
<span style="color:green; text-decoration:underline">`swordvistime2 0`</span>
`swordwaterfric1 0.0`
`swordwaterfric2 0.0`
<span style="color:green; text-decoration:underline">`swordwavepush1 1.5`</span>
<span style="color:green; text-decoration:underline">`swordwavepush2 1.5`</span>
`swordweight1 0.0`
`swordweight2 0.0`
<span style="color:red; text-decoration:line-through">`swordwhipdmg1`</span><span style="color:green; text-decoration:underline">`swordwhipdamage1`</span>` 0.8`
<span style="color:red; text-decoration:line-through">`swordwhipdmg2`</span><span style="color:green; text-decoration:underline">`swordwhipdamage2`</span>` 0.8 `<span style="color:red; text-decoration:line-through">`swordzdiv1 1`</span>
<span style="color:red; text-decoration:line-through">`swordzdiv2 1`</span>
`swordzooms 0`
`teamalphacolour 0x5F66FF`
`teamalphaname "alpha"`
`teambalance 1`
`teamdamage 1`
<span style="color:green; text-decoration:underline">`teamdamagescale 1.0`</span>
`teamenemyname "enemy"`
`teamkappacolour 0xFFD022`
`teamkappaname "kappa"`
<span style="color:green; text-decoration:underline">`teamkillban 3`</span>
<span style="color:green; text-decoration:underline">`teamkillkick 2`</span>
<span style="color:green; text-decoration:underline">`teamkilllock 4`</span>
`teamkillpenalty 2`
<span style="color:green; text-decoration:underline">`teamkillrestore 1`</span>
<span style="color:green; text-decoration:underline">`teamkilltime 5`</span>
<span style="color:green; text-decoration:underline">`teamkillwarn 5`</span>
`teamneutralcolour 0x90A090`
`teamneutralname "neutral"`
`teamomegacolour 0xFF4F44`
`teamsigmaname "sigma"`
`timelimit 10`
`trialdelay 500`
<span style="color:red; text-decoration:line-through">`triallimit 60000`</span><span style="color:green; text-decoration:underline">`trialghost 1`</span>
<span style="color:red; text-decoration:line-through">`trialstyle 0`</span><span style="color:green; text-decoration:underline">`trialmaps "cyanide hawk hinder neodrive purge testchamber"`</span>
`trialweapon 0`
<span style="color:green; text-decoration:underline">`varslock 4`</span>
<span style="color:green; text-decoration:underline">`vetolock 4`</span>
<span style="color:green; text-decoration:underline">`voteinterm 2`</span>
`votelimit 45000`
<span style="color:green; text-decoration:underline">`votelock 4`</span>
<span style="color:green; text-decoration:underline">`votelocktype 2`</span>
<span style="color:green; text-decoration:underline">`votestyle 2`</span>
<span style="color:green; text-decoration:underline">`votethreshold 0.5`</span>
<span style="color:green; text-decoration:underline">`votewait 2500`</span>
`wavepushscale 1.0`
<span style="color:red; text-decoration:line-through">`waveslowscale 0.5`</span><span style="color:green; text-decoration:underline">`wavestunscale 1.0`</span>
<span style="color:red; text-decoration:line-through">`weaponjamming 0`</span>
<span style="color:red; text-decoration:line-through">`weaponjamtime 1000`</span><span style="color:green; text-decoration:underline">`weaponinterrupts 56`</span>
`weaponswitchdelay 500`
<span style="color:red; text-decoration:line-through">`zoomlimit`</span><span style="color:green; text-decoration:underline">`zoomlimitmax 65`</span>
<span style="color:green; text-decoration:underline">`zoomlimitmin`</span>` 10`
`zoomlock 0`
`zoomlocktime 500`
`zoomtime 100`

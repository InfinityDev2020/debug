$nomention

$cooldown[5s;You can open crates again in %time%.]

$onlyIf[$getUserVar[commonkey]>=1;You better have to buy a common key first!]

$title[$username Opening a crate!]
$description[Opening common crate... $editIn[3s;$randomText[You got AUG-Storm from the crate!;You got M4A1-Blood tiger from the common crate!]]]
$image[https://cdn.discordapp.com/attachments/807316532467073054/810102919432896542/20210213_105856.jpg]

$if[$randomText[You got AUG-Storm from the common crate!;You got M4A1-Blood tiger from the common crate!]==You got AUG-Storm from the common crate!]

$setUserVar[augstorm;$sum[$getUserVar[augstorm];1]]

$setUserVar[commonskins;$sum[$getUserVar[commonskins];1]]

$if[$randomText[You got AUG-Storm from the common crate!;You got M4A1-Blood tiger from the common crate!]==You got M4A1-Blood tiger from the common crate!]

$image[https://cdn.discordapp.com/attachments/807316532467073054/810101553435377664/20210213_105346.jpg]

$setUserVar[m4bloodtiger;$sum[$getUserVar[m4bloodtiger];1]]

$setUserVar[rareskins;$sum[$getUserVar[rareskins];1]]

$endif
$endif

$setUserVar[commonkey;$sub[$getUserVar[commonkey];1]]

$color[C1C1C1]

(How can i make second image will appear when i get  rare skin?)

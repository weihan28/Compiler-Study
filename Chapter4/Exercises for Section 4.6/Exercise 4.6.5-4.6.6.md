---
excalidraw-plugin: parsed
tags:
  - excalidraw
---
==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Text Elements
Left Factor + left recursive elim: nothing changed

First(S) = {a, b}
First(A) = {ε}
First(B) = {ε}

Follow(S) = {$}
Follow(A) = {a, b}
Follow(B) = {a, b} ^H1j1khx8

non-terminal ^Q3GffWUL

input ^114sDs5t

S ^BQkWKh9v

A ^eUMAW9fQ

B ^I3U8TWs2

a ^jBSsZh8u

b ^5AxR9M4E

$ ^uurW34vz

S -> AaAb ^YdjqkPW7

S -> BbBa ^MjtgtKB3

A -> ε  ^tkVwCMlr

B -> ε ^XXYdZeBm

A -> ε  ^6j4tLc7V

B -> ε ^LBYFyiwJ

a LL(1) parsing table is constructed without any problems (no entries with 2 possible productions)
ie: this predictive parser (top-down) is created succesfully (predictive parsers dont need backtracking) ^UauoeDXX

LL(1)
predictive
parsing table ^pakfwqa7

S' -> . S
-----------
S -> . AaAb
S -> . BbBa
A -> . 
B -> .  ^kcp45J4x

both A -> . and B -> . will be reduced on 'a' and 'b'
Reduce-Reduce conflict ^E3S6U30k

Left Factor + left recursive elim:  ^XAzzenZ8

nothing to left factor ^7lDowyTR

A1, A2 = S, A

process A1:
    inline A1..A0: nothing to inline

    elim immediate left recursion:
        S -> AB
        B -> AB | ε

process A2:
    inline A1..A1: nothing to inline (no S non-terminals in A production)
    
    elim immediate left recursion:
        no left recursive A productions
 ^r2R7rqrR

S -> AB
B -> AB | ε
A -> a ^BKpuYrmt

Compute First + Follow: ^2S5ffSTg

First(S) = First(A) = {a}
First(B) = {ε} U First(A) = {a, ε}
First(A) = {a} ^PGSRIIUZ

Follow(S) = {$}
Follow(B) = Follow(S) = {$}
Follow(A) = First(B) U Follow(S) = {a, $} ^O9W8hXzT

non-terminal ^EKOa0b1H

input ^G7VtW3CG

S ^6Hogbesh

A ^anqGbIqo

B ^qseRSwNr

a ^9bYcbR7o

b ^zCGX7hfi

$ ^LIviW1AE

S -> AB ^6pdM6vh7

B -> AB ^Zv0t90VG

B -> ε ^M7Uz4go5

A -> a ^iPOJKoWM

First(S) = {a}
First(A) = {a} ^8G1ygjhT

Without left recursion elimination, it is not LL(1).
because S -> SA and S -> a will get filled into the same entry for input 'a'
for the non-terminal S in the LL(1) parsing table ^SFKDJVZM

without left recursion elimination: not LL(1) ^7fp4vsjs

with left recursion elimination: is LL(1) ^dSl1n8Zc

S' -> . S
-----------
S -> . SA 
S -> . A
A -> . a ^jPccM9hz

S' -> S . 
S -> S . A
----------- 
A -> . a ^BkVSFbo2

S -> A . ^4F2Wvws0

A -> a .  ^MjY2oT9r

S ^Fz2wQgjq

A ^s03Vh6bb

a ^Nk5LmxQA

Accept ^V9iY6Krj

$ ^qgaEzWDb

S -> SA .  ^NPpSps6G

A ^NBv96Um6

input ^urKuEnLa

a ^0VjkQ4HA

$ ^BPORJAuw

I0 ^HalvZ0oz

I1 ^uNVFn6lS

I2 ^TlEmJxu0

I3 ^lftxevVO

I4 ^sK6gAtCG

0 ^IfBpUPrp

1 ^DFpg6nzG

2 ^HoxOALP8

S ^fSV3beL4

A ^kgJOVYOt

0 ^GLF9RjvI

1 ^qX8ZFs73

2 ^EdDlhQOx

3 ^BPkUGq8O

4 ^7qtllvuc

1 ^MpF8ftuS

2 ^Zs8GKmY8

s3 ^OzFhhoHP

Accept ^TACY0qzJ

4 ^YyFMc7D4

a ^jRpzKYH9

s3 ^qndYqdnO

Follow(S) = {$, a}
Follow(A) = {$, a} ^48HX4aeO

r1 ^s796J56R

r1 ^tXuF8WGh

r2 ^8zPOBmsj

r2 ^dOx1rU4X

r0 ^swFv2x3w

r0 ^IeEIOZDR

state ^PiIl88wi

predictive parsing table ^LxOhZHB6

SLR(1) parsing table ^sNJmXRnC

# Embedded files
52ca63f4389ff884698fbdbba15191a1d333a158: [[Pasted Image 20240723212556_967.png]]
e8104027b1e67d1b11665205ac5f73d8633ef009: [[Pasted Image 20240723212603_917.png]]
b8ff33ef80642e75250b1d6b60866b9d26219bb0: [[Pasted Image 20240723213804_931.png]]
2a57aed57cc97125e67aff86a415ff1d58830420: [[Pasted Image 20240723214315_968.png]]
a4810a4f23a1bc300f69c820597e06d0b69c1c24: [[Pasted Image 20240724161816_400.png]]
8c9922bc8ef58272539f6a9ee731c8b5f62d1093: [[Pasted Image 20240725204115_227.png]]

%%
# Drawing
```json
{
	"type": "excalidraw",
	"version": 2,
	"source": "https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/2.1.7",
	"elements": [
		{
			"type": "image",
			"version": 186,
			"versionNonce": 1762794611,
			"index": "a1",
			"isDeleted": false,
			"id": "YN1HD53F_p66icHvOKOwN",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -789.2902507148153,
			"y": 1099.8915895578775,
			"strokeColor": "transparent",
			"backgroundColor": "transparent",
			"width": 1219.7702127659575,
			"height": 433,
			"seed": 1707590111,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721808860211,
			"link": null,
			"locked": false,
			"status": "pending",
			"fileId": "52ca63f4389ff884698fbdbba15191a1d333a158",
			"scale": [
				1,
				1
			]
		},
		{
			"type": "image",
			"version": 27,
			"versionNonce": 2146884127,
			"index": "a2",
			"isDeleted": false,
			"id": "ERO_bARVlCqoMCrSKTj8d",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -737.2045705379719,
			"y": -603.7891981686831,
			"strokeColor": "transparent",
			"backgroundColor": "transparent",
			"width": 1219.7702127659575,
			"height": 433,
			"seed": 1287108223,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721741161767,
			"link": null,
			"locked": false,
			"status": "pending",
			"fileId": "e8104027b1e67d1b11665205ac5f73d8633ef009",
			"scale": [
				1,
				1
			]
		},
		{
			"type": "text",
			"version": 235,
			"versionNonce": 1476245055,
			"index": "a4",
			"isDeleted": false,
			"id": "H1j1khx8",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -703.8634274751242,
			"y": -142.180757663647,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 494.0395812988281,
			"height": 225,
			"seed": 375415455,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721742142729,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Left Factor + left recursive elim: nothing changed\n\nFirst(S) = {a, b}\nFirst(A) = {ε}\nFirst(B) = {ε}\n\nFollow(S) = {$}\nFollow(A) = {a, b}\nFollow(B) = {a, b}",
			"rawText": "Left Factor + left recursive elim: nothing changed\n\nFirst(S) = {a, b}\nFirst(A) = {ε}\nFirst(B) = {ε}\n\nFollow(S) = {$}\nFollow(A) = {a, b}\nFollow(B) = {a, b}",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Left Factor + left recursive elim: nothing changed\n\nFirst(S) = {a, b}\nFirst(A) = {ε}\nFirst(B) = {ε}\n\nFollow(S) = {$}\nFollow(A) = {a, b}\nFollow(B) = {a, b}",
			"lineHeight": 1.25
		},
		{
			"type": "line",
			"version": 259,
			"versionNonce": 631697425,
			"index": "a6",
			"isDeleted": false,
			"id": "fMC7r05h6tTUhqoBfG4Mr",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -707.6871071415187,
			"y": 231.37129651416365,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 599.9547932326191,
			"height": 2.0504879408944134,
			"seed": 835791359,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721741685551,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					599.9547932326191,
					2.0504879408944134
				]
			]
		},
		{
			"type": "line",
			"version": 191,
			"versionNonce": 64960543,
			"index": "a7",
			"isDeleted": false,
			"id": "GowGJ8lwQeicKgSG-m6S4",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -574.89573564843,
			"y": 174.55276546733012,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.4890168745621395,
			"height": 295.7937631190443,
			"seed": 2039357425,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721741615794,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					1.4890168745621395,
					295.7937631190443
				]
			]
		},
		{
			"type": "text",
			"version": 52,
			"versionNonce": 902956639,
			"index": "a8",
			"isDeleted": false,
			"id": "Q3GffWUL",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -709.8824771052424,
			"y": 189.80884150583222,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 113.79989624023438,
			"height": 25,
			"seed": 1888061361,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721741548401,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "non-terminal",
			"rawText": "non-terminal",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "non-terminal",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 164,
			"versionNonce": 783110495,
			"index": "a9",
			"isDeleted": false,
			"id": "114sDs5t",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -369.5004847967481,
			"y": 186.658548413429,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 46.23994445800781,
			"height": 25,
			"seed": 1340113617,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721741633126,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "input",
			"rawText": "input",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "input",
			"lineHeight": 1.25
		},
		{
			"type": "line",
			"version": 391,
			"versionNonce": 546084223,
			"index": "aA",
			"isDeleted": false,
			"id": "lyqQBwaVscfM9ufYlHuW2",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -709.9661962950478,
			"y": 291.20772234914114,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 599.9547932326191,
			"height": 2.0504879408944134,
			"seed": 1937789823,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721741685551,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					599.9547932326191,
					2.0504879408944134
				]
			]
		},
		{
			"type": "line",
			"version": 315,
			"versionNonce": 1817232881,
			"index": "aB",
			"isDeleted": false,
			"id": "wC7x4-NwsVurmMLx6NpF9",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -712.7025444588202,
			"y": 346.80640908459753,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 599.9547932326191,
			"height": 2.0504879408944134,
			"seed": 862705521,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721741685551,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					599.9547932326191,
					2.0504879408944134
				]
			]
		},
		{
			"type": "line",
			"version": 339,
			"versionNonce": 1383828895,
			"index": "aC",
			"isDeleted": false,
			"id": "Lf8ApwQHaoDdZd99whrO5",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -713.216292915667,
			"y": 403.43826263172576,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 599.9547932326191,
			"height": 2.0504879408944134,
			"seed": 949103391,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721741685551,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					599.9547932326191,
					2.0504879408944134
				]
			]
		},
		{
			"type": "line",
			"version": 348,
			"versionNonce": 1325719505,
			"index": "aD",
			"isDeleted": false,
			"id": "F3Ew_I1niuZlYQ9nZIUeE",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -715.3368716524386,
			"y": 469.3104738970947,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 599.9547932326191,
			"height": 2.0504879408944134,
			"seed": 1656000593,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721741685551,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					599.9547932326191,
					2.0504879408944134
				]
			]
		},
		{
			"type": "text",
			"version": 48,
			"versionNonce": 1598598129,
			"index": "aE",
			"isDeleted": false,
			"id": "BQkWKh9v",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -672.9001657997377,
			"y": 305.88551540602083,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.159988403320312,
			"height": 25,
			"seed": 1099611409,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721741624951,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "S",
			"rawText": "S",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "S",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 99,
			"versionNonce": 1098283473,
			"index": "aF",
			"isDeleted": false,
			"id": "eUMAW9fQ",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -672.0806824889748,
			"y": 364.4339467967687,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.1199951171875,
			"height": 25,
			"seed": 1110728959,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721741627668,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "A",
			"rawText": "A",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "A",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 62,
			"versionNonce": 1248698961,
			"index": "aG",
			"isDeleted": false,
			"id": "I3U8TWs2",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -672.5918453461835,
			"y": 425.57064725814405,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.539993286132812,
			"height": 25,
			"seed": 1305227761,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721741629368,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "B",
			"rawText": "B",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "B",
			"lineHeight": 1.25
		},
		{
			"type": "line",
			"version": 149,
			"versionNonce": 62477713,
			"index": "aH",
			"isDeleted": false,
			"id": "UXm3Co_dYur3TIVgIYj1e",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -418.97122664388405,
			"y": 236.06986463362784,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.1230838249139765,
			"height": 235.93546566903535,
			"seed": 1955794417,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721741638940,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					2.1230838249139765,
					235.93546566903535
				]
			]
		},
		{
			"type": "line",
			"version": 253,
			"versionNonce": 2130830591,
			"index": "aI",
			"isDeleted": false,
			"id": "xWbh4FMZIcF8clf0T_DXv",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -261.5364455673618,
			"y": 234.4713383567946,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.1230838249139765,
			"height": 235.93546566903535,
			"seed": 886826321,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721741643284,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					2.1230838249139765,
					235.93546566903535
				]
			]
		},
		{
			"type": "line",
			"version": 191,
			"versionNonce": 1652031793,
			"index": "aJ",
			"isDeleted": false,
			"id": "aEnaXsCJ3Nspiod8YWtWI",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -108.9421621463814,
			"y": 233.66537787294183,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.1230838249139765,
			"height": 235.93546566903535,
			"seed": 505278783,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721741645794,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					2.1230838249139765,
					235.93546566903535
				]
			]
		},
		{
			"type": "text",
			"version": 3,
			"versionNonce": 777176575,
			"index": "aM",
			"isDeleted": false,
			"id": "jBSsZh8u",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -509.1496169171028,
			"y": 258.21991366388244,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.339996337890625,
			"height": 25,
			"seed": 2099308991,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721741669748,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "a",
			"rawText": "a",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "a",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 3,
			"versionNonce": 490481311,
			"index": "aN",
			"isDeleted": false,
			"id": "5AxR9M4E",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -350.88826214235735,
			"y": 256.92268944441736,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.159988403320312,
			"height": 25,
			"seed": 201060959,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721741670755,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "b",
			"rawText": "b",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "b",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 3,
			"versionNonce": 2113922641,
			"index": "aO",
			"isDeleted": false,
			"id": "uurW34vz",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -200.41025268440262,
			"y": 258.21991366388244,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16.05999755859375,
			"height": 25,
			"seed": 288986769,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721741675526,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "$",
			"rawText": "$",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "$",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 149,
			"versionNonce": 1673590077,
			"index": "aP",
			"isDeleted": false,
			"id": "YdjqkPW7",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -545.7011627256147,
			"y": 309.6089815845629,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 99.8199462890625,
			"height": 25,
			"seed": 530171249,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721809540220,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "S -> AaAb",
			"rawText": "S -> AaAb",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "S -> AaAb",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 94,
			"versionNonce": 131111857,
			"index": "aQ",
			"isDeleted": false,
			"id": "MjtgtKB3",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -388.58666457715674,
			"y": 310.77254551908163,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 102.65994262695312,
			"height": 25,
			"seed": 1122948063,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721741739810,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "S -> BbBa",
			"rawText": "S -> BbBa",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "S -> BbBa",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 78,
			"versionNonce": 167233695,
			"index": "aR",
			"isDeleted": false,
			"id": "tkVwCMlr",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -535.2176473819758,
			"y": 367.5748414711884,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 71.07997131347656,
			"height": 25,
			"seed": 1644870065,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721741750068,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "A -> ε ",
			"rawText": "A -> ε ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "A -> ε ",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 64,
			"versionNonce": 877394257,
			"index": "aS",
			"isDeleted": false,
			"id": "XXYdZeBm",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -533.3487506593228,
			"y": 427.48459292072357,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 62.499969482421875,
			"height": 25,
			"seed": 2075306513,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721741755518,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "B -> ε",
			"rawText": "B -> ε",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "B -> ε",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 111,
			"versionNonce": 220052735,
			"index": "aT",
			"isDeleted": false,
			"id": "6j4tLc7V",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -380.5559219069595,
			"y": 366.0670505973236,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 71.07997131347656,
			"height": 25,
			"seed": 2120707295,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721741753401,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "A -> ε ",
			"rawText": "A -> ε ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "A -> ε ",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 122,
			"versionNonce": 1424155089,
			"index": "aW",
			"isDeleted": false,
			"id": "LBYFyiwJ",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -381.4689737015393,
			"y": 426.12056333321675,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 62.499969482421875,
			"height": 25,
			"seed": 2020120849,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721741758092,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "B -> ε",
			"rawText": "B -> ε",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "B -> ε",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 329,
			"versionNonce": 629036767,
			"index": "aZ",
			"isDeleted": false,
			"id": "UauoeDXX",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -731.3026604216034,
			"y": 517.4411271373756,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1013.55908203125,
			"height": 50,
			"seed": 1368259583,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721742047727,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "a LL(1) parsing table is constructed without any problems (no entries with 2 possible productions)\nie: this predictive parser (top-down) is created succesfully (predictive parsers dont need backtracking)",
			"rawText": "a LL(1) parsing table is constructed without any problems (no entries with 2 possible productions)\nie: this predictive parser (top-down) is created succesfully (predictive parsers dont need backtracking)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "a LL(1) parsing table is constructed without any problems (no entries with 2 possible productions)\nie: this predictive parser (top-down) is created succesfully (predictive parsers dont need backtracking)",
			"lineHeight": 1.25
		},
		{
			"type": "image",
			"version": 189,
			"versionNonce": 419847665,
			"index": "aa",
			"isDeleted": false,
			"id": "g2T-Xbz3ryt8v5rRWtGFO",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1551.057389443748,
			"y": 71.23725081148984,
			"strokeColor": "transparent",
			"backgroundColor": "transparent",
			"width": 400.5840326489454,
			"height": 85.06610731927412,
			"seed": 1679884145,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721741957968,
			"link": null,
			"locked": false,
			"status": "pending",
			"fileId": "b8ff33ef80642e75250b1d6b60866b9d26219bb0",
			"scale": [
				1,
				1
			]
		},
		{
			"type": "freedraw",
			"version": 179,
			"versionNonce": 336482097,
			"index": "ae",
			"isDeleted": false,
			"id": "evA993LpKoyA7qRCuMFkp",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -734.1730059605673,
			"y": -120.19886494134136,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 78.13756187007812,
			"height": 686.2928279506084,
			"seed": 1352562513,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721741968617,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-2.1821725329401715,
					-2.093164005041615
				],
				[
					-3.273258799410314,
					-2.878086955085678
				],
				[
					-4.44825809949009,
					-3.6630099051297407
				],
				[
					-5.707170433179613,
					-4.360767378400965
				],
				[
					-6.8821697332593885,
					-4.971250960127236
				],
				[
					-8.728581716988742,
					-5.843393594330223
				],
				[
					-9.316081367028687,
					-6.192272330965807
				],
				[
					-9.819667983458885,
					-6.453877176056494
				],
				[
					-10.323254599889083,
					-6.628316544374286
				],
				[
					-10.910754249928914,
					-6.715590435919239
				],
				[
					-11.582166933578492,
					-6.628316544374286
				],
				[
					-13.176839816478832,
					-5.930613278489091
				],
				[
					-14.267926082948975,
					-5.3201296967628195
				],
				[
					-15.526838416638384,
					-4.535152539332728
				],
				[
					-16.953576817547287,
					-3.6630099051297407
				],
				[
					-18.46433666683788,
					-2.703647586767829
				],
				[
					-21.737487051476137,
					-0.6977574732712242
				],
				[
					-23.416181382758168,
					0.436098420794508
				],
				[
					-25.17868033287789,
					1.7442310610198888
				],
				[
					-28.70356981834516,
					4.709591907650463
				],
				[
					-31.89291558414584,
					8.634206657870834
				],
				[
					-33.15182791783525,
					11.163469083706957
				],
				[
					-34.15900115069576,
					14.128775722951502
				],
				[
					-34.91432686795497,
					17.617400467149423
				],
				[
					-35.41791348438517,
					21.716454585687586
				],
				[
					-35.66976099998635,
					26.513266177497087
				],
				[
					-35.66976099998635,
					38.11283368199855
				],
				[
					-35.501826517994914,
					44.74115022637278
				],
				[
					-35.25008741716579,
					51.805565191541575
				],
				[
					-34.9982399015646,
					59.13158500180094
				],
				[
					-34.662587767125956,
					66.71926386453714
				],
				[
					-33.73932756787519,
					82.33066580341784
				],
				[
					-32.56432826779542,
					97.94212194968469
				],
				[
					-31.976828617755473,
					105.52980081242077
				],
				[
					-31.473242001325275,
					112.85587483006628
				],
				[
					-30.969763799667135,
					119.92023558784905
				],
				[
					-30.550090216846684,
					126.8102111847
				],
				[
					-30.2982427012455,
					133.35130804491536
				],
				[
					-30.13041663402612,
					145.64857881530196
				],
				[
					-30.2982427012455,
					151.40480693285934
				],
				[
					-30.717916284066064,
					156.89932179055398
				],
				[
					-31.305415934105895,
					162.30661696408964
				],
				[
					-32.06074165136522,
					167.53947276930745
				],
				[
					-32.98400185061587,
					172.77243698929743
				],
				[
					-35.501826517994914,
					183.2382028071192
				],
				[
					-36.92867333367576,
					188.55822408910996
				],
				[
					-38.523237801804044,
					193.79118830909994
				],
				[
					-41.79649660121436,
					204.1696802353768
				],
				[
					-43.3911694841147,
					209.14093119550392
				],
				[
					-46.49649380153346,
					218.8218282706677
				],
				[
					-47.83931916883262,
					223.4440920793872
				],
				[
					-49.09823150252214,
					227.80485945778815
				],
				[
					-50.35725225098372,
					231.99118746787127
				],
				[
					-51.532251551063496,
					236.00307610963665
				],
				[
					-52.62322940276147,
					239.84052538308418
				],
				[
					-53.71442408400367,
					243.5907007649867
				],
				[
					-57.07148750225167,
					253.62047657678607
				],
				[
					-58.1625737687217,
					256.4113980550989
				],
				[
					-59.25366003519184,
					258.853332382004
				],
				[
					-60.344746301661985,
					260.94649638704556
				],
				[
					-61.435832568132014,
					262.69078165545153
				],
				[
					-62.44300580099241,
					264.17335366399465
				],
				[
					-64.20550475111213,
					266.3537915605812
				],
				[
					-64.87680901998965,
					267.1388229253974
				],
				[
					-65.46430867002948,
					267.74930650712366
				],
				[
					-65.96800370123185,
					268.2725161973049
				],
				[
					-66.30365583567061,
					268.70856041071346
				],
				[
					-66.47148190288999,
					269.0575475621211
				],
				[
					-66.47148190288999,
					269.92963598893806
				],
				[
					-65.96800370123185,
					271.4994818890262
				],
				[
					-65.46430867002948,
					272.546009684161
				],
				[
					-64.87680901998965,
					273.7670852623856
				],
				[
					-64.12148330273033,
					275.2497656857009
				],
				[
					-63.198331518251734,
					277.0812164308797
				],
				[
					-62.10724525178159,
					279.1742720211492
				],
				[
					-59.67333361801241,
					283.97119202773064
				],
				[
					-56.987574468641924,
					289.727365937902
				],
				[
					-55.7286621349524,
					292.8671661528504
				],
				[
					-54.553662834872625,
					296.3556282748902
				],
				[
					-53.54648960201223,
					300.1059120715649
				],
				[
					-52.70725085114327,
					304.11780071333015
				],
				[
					-52.11975120110344,
					308.3912942001861
				],
				[
					-51.700077618282876,
					317.54887317039646
				],
				[
					-51.867903685502256,
					322.4328502389788
				],
				[
					-52.28757726832282,
					327.49126667587876
				],
				[
					-52.87507691836265,
					332.72423089586874
				],
				[
					-53.63040263562198,
					338.0442521778595
				],
				[
					-54.46974980126299,
					343.45165576616733
				],
				[
					-56.40007481860209,
					354.61512484987423
				],
				[
					-57.323226603080684,
					360.3712987600455
				],
				[
					-58.24648680233145,
					366.21474656176173
				],
				[
					-59.08583396797246,
					372.14525142547876
				],
				[
					-59.92507271884142,
					378.0759731187399
				],
				[
					-60.6805068508728,
					384.09375187400184
				],
				[
					-61.435832568132014,
					390.1986961060367
				],
				[
					-62.19115828539134,
					396.3909142296164
				],
				[
					-63.701809719909875,
					409.0370637366387
				],
				[
					-64.45724385194126,
					415.40382964330837
				],
				[
					-65.12865653559084,
					421.8577610267509
				],
				[
					-65.80006921924041,
					428.31158399542124
				],
				[
					-66.47148190288999,
					434.8526808556366
				],
				[
					-67.14300300131163,
					441.39388613062414
				],
				[
					-68.3180023013914,
					454.38880595950985
				],
				[
					-69.57691463508093,
					467.2965603116227
				],
				[
					-70.2483273187305,
					473.66321780352035
				],
				[
					-70.91974000238008,
					480.02998371019004
				],
				[
					-71.59115268602966,
					486.30936731054254
				],
				[
					-73.01789108693845,
					498.51936418938425
				],
				[
					-74.44473790261941,
					510.0318204244989
				],
				[
					-75.11615058626899,
					515.5262810748075
				],
				[
					-75.70365023630893,
					520.8464107715704
				],
				[
					-76.29114988634876,
					526.0792665767881
				],
				[
					-76.79473650277896,
					531.1376830136883
				],
				[
					-77.21441008559952,
					536.1089339738155
				],
				[
					-77.80190973563947,
					545.7898310489793
				],
				[
					-77.96973580285874,
					550.4123116872429
				],
				[
					-78.05364883646848,
					554.8601361276446
				],
				[
					-78.13756187007812,
					559.1337380292728
				],
				[
					-78.13756187007812,
					563.2327921478109
				],
				[
					-78.13756187007812,
					567.1575153128033
				],
				[
					-77.96973580285874,
					574.5707005998356
				],
				[
					-77.71788828725767,
					581.4606761966866
				],
				[
					-77.55006222003828,
					584.7748073651808
				],
				[
					-77.46614918642854,
					587.9146075801291
				],
				[
					-77.29832311920916,
					590.9671339035326
				],
				[
					-77.13038863721772,
					593.8451124438461
				],
				[
					-76.96256256999834,
					596.636033922159
				],
				[
					-76.79473650277896,
					599.2525160321538
				],
				[
					-76.62691043555958,
					604.2237669922811
				],
				[
					-76.54288898717789,
					606.5785358424134
				],
				[
					-76.37506291995851,
					611.2880735426779
				],
				[
					-76.29114988634876,
					613.6429508075821
				],
				[
					-76.20723685273913,
					615.9977196577145
				],
				[
					-76.03941078551975,
					618.3524885078466
				],
				[
					-75.70365023630893,
					623.0621346228831
				],
				[
					-75.53582416908955,
					625.4169034730153
				],
				[
					-75.28408506826042,
					627.6845068463747
				],
				[
					-75.03223755265935,
					629.9521102197341
				],
				[
					-74.6965854182206,
					632.1324397015485
				],
				[
					-74.36082486900978,
					634.312877598135
				],
				[
					-74.02506431979884,
					636.4059331884046
				],
				[
					-73.60539073697839,
					638.499097193446
				],
				[
					-72.59832591889005,
					642.5109858352114
				],
				[
					-72.09473930245986,
					644.429602057163
				],
				[
					-71.50723965241991,
					646.2612696318861
				],
				[
					-70.91974000238008,
					648.005554900292
				],
				[
					-70.2483273187305,
					649.662566277153
				],
				[
					-69.57691463508093,
					651.2325205920133
				],
				[
					-68.15006781939996,
					654.2850469154168
				],
				[
					-67.39474210214064,
					655.6804534471871
				],
				[
					-66.63930797010926,
					656.9885860874124
				],
				[
					-65.88398225285005,
					658.2095532508649
				],
				[
					-65.12865653559084,
					659.4307372438618
				],
				[
					-64.37333081833151,
					660.5644305157693
				],
				[
					-62.69474490182154,
					663.0064732574465
				],
				[
					-61.01615898531156,
					665.4485159991236
				],
				[
					-60.176811819670434,
					666.6694831625762
				],
				[
					-59.337573068801476,
					667.9777242175737
				],
				[
					-58.414421284322884,
					669.2859652725713
				],
				[
					-57.40724805146249,
					670.5942063275688
				],
				[
					-55.30898855213195,
					673.2105800227916
				],
				[
					-54.21790228566181,
					674.4316556010162
				],
				[
					-53.04290298558203,
					675.5653488729238
				],
				[
					-51.95192513388406,
					676.6119850828306
				],
				[
					-50.86073045264186,
					677.4840735096475
				],
				[
					-49.85366563455352,
					678.2689964596916
				],
				[
					-48.846492401693126,
					678.966753932963
				],
				[
					-47.251819518792786,
					679.5772375146892
				],
				[
					-46.748341317134646,
					679.2283587780535
				],
				[
					-46.49649380153346,
					678.5307097195544
				],
				[
					-46.748341317134646,
					677.4840735096475
				],
				[
					-47.41975400078422,
					676.1759408694222
				],
				[
					-48.510731852482195,
					674.7804259228797
				],
				[
					-49.685731152562084,
					673.0361406544739
				],
				[
					-50.776925833804285,
					670.9429766494322
				],
				[
					-51.532251551063496,
					668.5882077993001
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.054901961237192154,
				0.35686275362968445,
				0.4745098054409027,
				0.5607843399047852,
				0.6235294342041016,
				0.6666666865348816,
				0.7215686440467834,
				0.7372549176216125,
				0.7490196228027344,
				0.7568627595901489,
				0.7607843279838562,
				0.7686274647712708,
				0.7803921699523926,
				0.7882353067398071,
				0.7960784435272217,
				0.8039215803146362,
				0.8156862854957581,
				0.8392156958580017,
				0.8509804010391235,
				0.8666666746139526,
				0.8784313797950745,
				0.9058823585510254,
				0.9137254953384399,
				0.9215686321258545,
				0.929411768913269,
				0.9333333373069763,
				0.9411764740943909,
				0.9529411792755127,
				0.95686274766922,
				0.9607843160629272,
				0.9647058844566345,
				0.9647058844566345,
				0.9725490212440491,
				0.9764705896377563,
				0.9803921580314636,
				0.9803921580314636,
				0.9843137264251709,
				0.9843137264251709,
				0.9843137264251709,
				0.9882352948188782,
				0.9960784316062927,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				1,
				0.9254902005195618,
				0.8392156958580017,
				0.7137255072593689,
				0.5686274766921997,
				0.41960784792900085,
				0.27450981736183167,
				0.1411764770746231,
				0.0470588244497776,
				0
			]
		},
		{
			"type": "text",
			"version": 99,
			"versionNonce": 2093466737,
			"index": "ah",
			"isDeleted": false,
			"id": "pakfwqa7",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -939.3984051978456,
			"y": 129.57254739734935,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 127.39988708496094,
			"height": 75,
			"seed": 178393951,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721742064669,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "LL(1)\npredictive\nparsing table",
			"rawText": "LL(1)\npredictive\nparsing table",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "LL(1)\npredictive\nparsing table",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 89,
			"versionNonce": 601019185,
			"index": "ai",
			"isDeleted": false,
			"id": "kcp45J4x",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -738.6094284740681,
			"y": 810.2454450135629,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 118.13993835449219,
			"height": 150,
			"seed": 333883327,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721798704481,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "S' -> . S\n-----------\nS -> . AaAb\nS -> . BbBa\nA -> . \nB -> . ",
			"rawText": "S' -> . S\n-----------\nS -> . AaAb\nS -> . BbBa\nA -> . \nB -> . ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "S' -> . S\n-----------\nS -> . AaAb\nS -> . BbBa\nA -> . \nB -> . ",
			"lineHeight": 1.25
		},
		{
			"type": "image",
			"version": 36,
			"versionNonce": 266327839,
			"index": "ap",
			"isDeleted": false,
			"id": "kZVWNJgBrUCYKOB3lHlz8",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -715.3023658266071,
			"y": 649.6709134517337,
			"strokeColor": "transparent",
			"backgroundColor": "transparent",
			"width": 212.00000000000003,
			"height": 98,
			"seed": 1871373009,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721742186548,
			"link": null,
			"locked": false,
			"status": "pending",
			"fileId": "2a57aed57cc97125e67aff86a415ff1d58830420",
			"scale": [
				1,
				1
			]
		},
		{
			"type": "rectangle",
			"version": 28,
			"versionNonce": 497463217,
			"index": "b0O",
			"isDeleted": false,
			"id": "vO4S0bLCn-ZA4SSOSBYD3",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -752.6314201983332,
			"y": 908.8326697889942,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 101.52261165895789,
			"height": 59.495199010755414,
			"seed": 675025023,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3
			},
			"boundElements": [],
			"updated": 1721798710242,
			"link": null,
			"locked": false
		},
		{
			"type": "text",
			"version": 169,
			"versionNonce": 1484667857,
			"index": "b0P",
			"isDeleted": false,
			"id": "E3S6U30k",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -629.7773674516944,
			"y": 913.4487204342789,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 513.0196533203125,
			"height": 50,
			"seed": 964137361,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721798749654,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "both A -> . and B -> . will be reduced on 'a' and 'b'\nReduce-Reduce conflict",
			"rawText": "both A -> . and B -> . will be reduced on 'a' and 'b'\nReduce-Reduce conflict",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "both A -> . and B -> . will be reduced on 'a' and 'b'\nReduce-Reduce conflict",
			"lineHeight": 1.25
		},
		{
			"type": "image",
			"version": 197,
			"versionNonce": 404530867,
			"index": "b0V",
			"isDeleted": false,
			"id": "UiL5ESVcU2kkLgtAUDIVM",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 243.0614599770754,
			"y": 2222.3642567294582,
			"strokeColor": "transparent",
			"backgroundColor": "transparent",
			"width": 461.5355525362313,
			"height": 232.71354166666637,
			"seed": 249561459,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810688861,
			"link": null,
			"locked": false,
			"status": "pending",
			"fileId": "a4810a4f23a1bc300f69c820597e06d0b69c1c24",
			"scale": [
				1,
				1
			]
		},
		{
			"type": "text",
			"version": 483,
			"versionNonce": 1700409107,
			"index": "b0w2",
			"isDeleted": false,
			"id": "XAzzenZ8",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -733.0652366542192,
			"y": 2093.09420289838,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 343.75970458984375,
			"height": 25,
			"seed": 1819447837,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Left Factor + left recursive elim: ",
			"rawText": "Left Factor + left recursive elim: ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Left Factor + left recursive elim: ",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 337,
			"versionNonce": 1475493789,
			"index": "b0w4",
			"isDeleted": false,
			"id": "7lDowyTR",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -646.8619746181887,
			"y": 2132.9153106922545,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 219.01980590820312,
			"height": 25,
			"seed": 864476307,
			"groupIds": [
				"hy5EkX2Z1knimNGd_sGZs"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "nothing to left factor",
			"rawText": "nothing to left factor",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "nothing to left factor",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 683,
			"versionNonce": 118019251,
			"index": "b0w6",
			"isDeleted": false,
			"id": "r2R7rqrR",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -642.3993520818728,
			"y": 2205.192716619825,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 665.4395141601562,
			"height": 375,
			"seed": 373747261,
			"groupIds": [
				"hy5EkX2Z1knimNGd_sGZs"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "A1, A2 = S, A\n\nprocess A1:\n    inline A1..A0: nothing to inline\n\n    elim immediate left recursion:\n        S -> AB\n        B -> AB | ε\n\nprocess A2:\n    inline A1..A1: nothing to inline (no S non-terminals in A production)\n    \n    elim immediate left recursion:\n        no left recursive A productions\n",
			"rawText": "A1, A2 = S, A\n\nprocess A1:\n    inline A1..A0: nothing to inline\n\n    elim immediate left recursion:\n        S -> AB\n        B -> AB | ε\n\nprocess A2:\n    inline A1..A1: nothing to inline (no S non-terminals in A production)\n    \n    elim immediate left recursion:\n        no left recursive A productions\n",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "A1, A2 = S, A\n\nprocess A1:\n    inline A1..A0: nothing to inline\n\n    elim immediate left recursion:\n        S -> AB\n        B -> AB | ε\n\nprocess A2:\n    inline A1..A1: nothing to inline (no S non-terminals in A production)\n    \n    elim immediate left recursion:\n        no left recursive A productions\n",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 321,
			"versionNonce": 1780630525,
			"index": "b0w8",
			"isDeleted": false,
			"id": "BKpuYrmt",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -652.5851140300949,
			"y": 2597.187256342012,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 177.7154998779297,
			"height": 117.41687823093261,
			"seed": 1728853661,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"fontSize": 31.311167528248692,
			"fontFamily": 1,
			"text": "S -> AB\nB -> AB | ε\nA -> a",
			"rawText": "S -> AB\nB -> AB | ε\nA -> a",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "S -> AB\nB -> AB | ε\nA -> a",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 296,
			"versionNonce": 1930544723,
			"index": "b0wA",
			"isDeleted": false,
			"id": "2S5ffSTg",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -720.6265393603237,
			"y": 2743.7488861058446,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 230.3798065185547,
			"height": 25,
			"seed": 1664250131,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Compute First + Follow:",
			"rawText": "Compute First + Follow:",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Compute First + Follow:",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 359,
			"versionNonce": 1418902621,
			"index": "b0wC",
			"isDeleted": false,
			"id": "PGSRIIUZ",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -666.4692129719799,
			"y": 2789.8819622699657,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 341.2997741699219,
			"height": 75,
			"seed": 782098003,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "First(S) = First(A) = {a}\nFirst(B) = {ε} U First(A) = {a, ε}\nFirst(A) = {a}",
			"rawText": "First(S) = First(A) = {a}\nFirst(B) = {ε} U First(A) = {a, ε}\nFirst(A) = {a}",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "First(S) = First(A) = {a}\nFirst(B) = {ε} U First(A) = {a, ε}\nFirst(A) = {a}",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 320,
			"versionNonce": 4948979,
			"index": "b0wG",
			"isDeleted": false,
			"id": "O9W8hXzT",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -664.1040669598972,
			"y": 2894.073923326362,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 409.17974853515625,
			"height": 75,
			"seed": 1418383091,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Follow(S) = {$}\nFollow(B) = Follow(S) = {$}\nFollow(A) = First(B) U Follow(S) = {a, $}",
			"rawText": "Follow(S) = {$}\nFollow(B) = Follow(S) = {$}\nFollow(A) = First(B) U Follow(S) = {a, $}",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Follow(S) = {$}\nFollow(B) = Follow(S) = {$}\nFollow(A) = First(B) U Follow(S) = {a, $}",
			"lineHeight": 1.25
		},
		{
			"type": "line",
			"version": 511,
			"versionNonce": 521480381,
			"index": "b0wI",
			"isDeleted": false,
			"id": "B8bvkRuIHcxKD9PS81Ydo",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -657.367204004988,
			"y": 3065.0142294258285,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 599.9547932326191,
			"height": 2.0504879408944134,
			"seed": 90558963,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					599.9547932326191,
					2.0504879408944134
				]
			]
		},
		{
			"type": "line",
			"version": 443,
			"versionNonce": 1723633043,
			"index": "b0wK",
			"isDeleted": false,
			"id": "sVPp3bXBGLa1p3mtEJwDi",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -524.5758325118998,
			"y": 3008.195698378995,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.4890168745621395,
			"height": 295.7937631190443,
			"seed": 794631059,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					1.4890168745621395,
					295.7937631190443
				]
			]
		},
		{
			"type": "text",
			"version": 304,
			"versionNonce": 1531644189,
			"index": "b0wO",
			"isDeleted": false,
			"id": "EKOa0b1H",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -659.5625739687123,
			"y": 3023.4517744174973,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 113.79989624023438,
			"height": 25,
			"seed": 1526346035,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "non-terminal",
			"rawText": "non-terminal",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "non-terminal",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 416,
			"versionNonce": 429613875,
			"index": "b0wQ",
			"isDeleted": false,
			"id": "G7VtW3CG",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -319.1805816602175,
			"y": 3020.301481325094,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 46.23994445800781,
			"height": 25,
			"seed": 1772327635,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "input",
			"rawText": "input",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "input",
			"lineHeight": 1.25
		},
		{
			"type": "line",
			"version": 643,
			"versionNonce": 1789255037,
			"index": "b0wS",
			"isDeleted": false,
			"id": "jFEIsMenIxjowQP2jVGYP",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -659.6462931585177,
			"y": 3124.850655260806,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 599.9547932326191,
			"height": 2.0504879408944134,
			"seed": 1274003571,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					599.9547932326191,
					2.0504879408944134
				]
			]
		},
		{
			"type": "line",
			"version": 567,
			"versionNonce": 1632535763,
			"index": "b0wV",
			"isDeleted": false,
			"id": "ws7V0EO9kCml7IwTWT6lx",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -662.3826413222898,
			"y": 3180.449341996263,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 599.9547932326191,
			"height": 2.0504879408944134,
			"seed": 463813139,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					599.9547932326191,
					2.0504879408944134
				]
			]
		},
		{
			"type": "line",
			"version": 591,
			"versionNonce": 73868765,
			"index": "b0wX",
			"isDeleted": false,
			"id": "DWiuacbGCM_c800mTvpMm",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -662.8963897791366,
			"y": 3237.081195543391,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 599.9547932326191,
			"height": 2.0504879408944134,
			"seed": 1975156659,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					599.9547932326191,
					2.0504879408944134
				]
			]
		},
		{
			"type": "line",
			"version": 600,
			"versionNonce": 896299635,
			"index": "b0wZ",
			"isDeleted": false,
			"id": "TPMzokqRe-z9v5M-q-KAk",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -665.0169685159083,
			"y": 3302.9534068087596,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 599.9547932326191,
			"height": 2.0504879408944134,
			"seed": 341184851,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					599.9547932326191,
					2.0504879408944134
				]
			]
		},
		{
			"type": "text",
			"version": 300,
			"versionNonce": 2074108477,
			"index": "b0wd",
			"isDeleted": false,
			"id": "6Hogbesh",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -622.5802626632069,
			"y": 3139.5284483176856,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.159988403320312,
			"height": 25,
			"seed": 684617459,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "S",
			"rawText": "S",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "S",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 351,
			"versionNonce": 1455139859,
			"index": "b0wf",
			"isDeleted": false,
			"id": "anqGbIqo",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -621.7607793524442,
			"y": 3198.076879708434,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.1199951171875,
			"height": 25,
			"seed": 1974081683,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "A",
			"rawText": "A",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "A",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 314,
			"versionNonce": 1160975005,
			"index": "b0wh",
			"isDeleted": false,
			"id": "qseRSwNr",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -622.2719422096527,
			"y": 3259.2135801698096,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.539993286132812,
			"height": 25,
			"seed": 681545267,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "B",
			"rawText": "B",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "B",
			"lineHeight": 1.25
		},
		{
			"type": "line",
			"version": 401,
			"versionNonce": 691188147,
			"index": "b0wl",
			"isDeleted": false,
			"id": "coqCkamzdikPgGiI19E-p",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -368.6513235073537,
			"y": 3069.712797545293,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.1230838249139765,
			"height": 235.93546566903535,
			"seed": 1955942355,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					2.1230838249139765,
					235.93546566903535
				]
			]
		},
		{
			"type": "line",
			"version": 505,
			"versionNonce": 1037088509,
			"index": "b0wn",
			"isDeleted": false,
			"id": "HyolN2zRumt5H0jWNBaKB",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -211.21654243083162,
			"y": 3068.1142712684596,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.1230838249139765,
			"height": 235.93546566903535,
			"seed": 1805770099,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					2.1230838249139765,
					235.93546566903535
				]
			]
		},
		{
			"type": "line",
			"version": 443,
			"versionNonce": 1308099411,
			"index": "b0wp",
			"isDeleted": false,
			"id": "o3HpgujTmn714-go9EvO0",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -58.62225900985072,
			"y": 3067.308310784607,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 2.1230838249139765,
			"height": 235.93546566903535,
			"seed": 420198163,
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					2.1230838249139765,
					235.93546566903535
				]
			]
		},
		{
			"type": "text",
			"version": 256,
			"versionNonce": 2089476005,
			"index": "b0wt",
			"isDeleted": false,
			"id": "9bYcbR7o",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -458.8297137805723,
			"y": 3091.992791569382,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.339996337890625,
			"height": 25,
			"seed": 1531534515,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721981454225,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "a",
			"rawText": "a",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "a",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 255,
			"versionNonce": 2103582963,
			"index": "b0wv",
			"isDeleted": false,
			"id": "zCGX7hfi",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -300.56835900582723,
			"y": 3090.5656223560827,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 10.159988403320312,
			"height": 25,
			"seed": 2114014803,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "b",
			"rawText": "b",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "b",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 255,
			"versionNonce": 436394941,
			"index": "b0wx",
			"isDeleted": false,
			"id": "LIviW1AE",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -150.09034954787217,
			"y": 3091.8628465755473,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16.05999755859375,
			"height": 25,
			"seed": 336202739,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "$",
			"rawText": "$",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "$",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 294,
			"versionNonce": 553093779,
			"index": "b0x",
			"isDeleted": false,
			"id": "6pdM6vh7",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -485.4608053883228,
			"y": 3143.2744003363814,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 77.73995971679688,
			"height": 25,
			"seed": 658706525,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "S -> AB",
			"rawText": "S -> AB",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "S -> AB",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 213,
			"versionNonce": 873094173,
			"index": "b0y",
			"isDeleted": false,
			"id": "Zv0t90VG",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -484.4716714149997,
			"y": 3260.971967484358,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 80.11996459960938,
			"height": 25,
			"seed": 1342081107,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "B -> AB",
			"rawText": "B -> AB",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "B -> AB",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 238,
			"versionNonce": 762232883,
			"index": "b0z",
			"isDeleted": false,
			"id": "M7Uz4go5",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -173.97736056626786,
			"y": 3265.200398024346,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 62.499969482421875,
			"height": 25,
			"seed": 855861661,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "B -> ε",
			"rawText": "B -> ε",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "B -> ε",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 210,
			"versionNonce": 906154109,
			"index": "b10",
			"isDeleted": false,
			"id": "iPOJKoWM",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -483.9466334765532,
			"y": 3199.6222219446454,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 64.37997436523438,
			"height": 25,
			"seed": 1215621981,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810691783,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "A -> a",
			"rawText": "A -> a",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "A -> a",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 104,
			"versionNonce": 394771770,
			"index": "b11",
			"isDeleted": false,
			"id": "8G1ygjhT",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -741.4982116667755,
			"y": 1622.3159026220646,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 141.8599090576172,
			"height": 50,
			"seed": 934386675,
			"groupIds": [
				"UITRwFWVNs-eDMJtDMS_J"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911546225,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "First(S) = {a}\nFirst(A) = {a}",
			"rawText": "First(S) = {a}\nFirst(A) = {a}",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "First(S) = {a}\nFirst(A) = {a}",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 254,
			"versionNonce": 550503930,
			"index": "b12",
			"isDeleted": false,
			"id": "SFKDJVZM",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -736.2976197471695,
			"y": 1752.330700612213,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 751.9593505859375,
			"height": 75,
			"seed": 695667411,
			"groupIds": [
				"UITRwFWVNs-eDMJtDMS_J"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911546225,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Without left recursion elimination, it is not LL(1).\nbecause S -> SA and S -> a will get filled into the same entry for input 'a'\nfor the non-terminal S in the LL(1) parsing table",
			"rawText": "Without left recursion elimination, it is not LL(1).\nbecause S -> SA and S -> a will get filled into the same entry for input 'a'\nfor the non-terminal S in the LL(1) parsing table",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Without left recursion elimination, it is not LL(1).\nbecause S -> SA and S -> a will get filled into the same entry for input 'a'\nfor the non-terminal S in the LL(1) parsing table",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 116,
			"versionNonce": 206631837,
			"index": "b16",
			"isDeleted": false,
			"id": "7fp4vsjs",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -745.6572322240083,
			"y": 1529.21139248134,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 863.8753051757812,
			"height": 51.26964224763572,
			"seed": 277782963,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810688861,
			"link": null,
			"locked": false,
			"fontSize": 41.01571379810858,
			"fontFamily": 1,
			"text": "without left recursion elimination: not LL(1)",
			"rawText": "without left recursion elimination: not LL(1)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "without left recursion elimination: not LL(1)",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 226,
			"versionNonce": 1411342515,
			"index": "b17",
			"isDeleted": false,
			"id": "dSl1n8Zc",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -733.9237232806088,
			"y": 1989.2102168938388,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 760.8992309570312,
			"height": 51.26964224763572,
			"seed": 589409587,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721810688861,
			"link": null,
			"locked": false,
			"fontSize": 41.01571379810858,
			"fontFamily": 1,
			"text": "with left recursion elimination: is LL(1)",
			"rawText": "with left recursion elimination: is LL(1)",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "with left recursion elimination: is LL(1)",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 218,
			"versionNonce": 1905071398,
			"index": "b1I",
			"isDeleted": false,
			"id": "jPccM9hz",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -680.8381623928719,
			"y": 3626.64972232738,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 100.83995056152344,
			"height": 125,
			"seed": 23406077,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "3uYPAZHgJkDJFXZXeykA-",
					"type": "arrow"
				},
				{
					"id": "2VvNqkkoRspS0rnBJU2pz",
					"type": "arrow"
				},
				{
					"id": "ErY8bRrynSLjZzuA-Qj2j",
					"type": "arrow"
				}
			],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "S' -> . S\n-----------\nS -> . SA \nS -> . A\nA -> . a",
			"rawText": "S' -> . S\n-----------\nS -> . SA \nS -> . A\nA -> . a",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "S' -> . S\n-----------\nS -> . SA \nS -> . A\nA -> . a",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 367,
			"versionNonce": 156678202,
			"index": "b1K",
			"isDeleted": false,
			"id": "BkVSFbo2",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -393.0212220019064,
			"y": 3597.064535371208,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 100.83995056152344,
			"height": 100,
			"seed": 2066498141,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "3uYPAZHgJkDJFXZXeykA-",
					"type": "arrow"
				},
				{
					"id": "qa7Hw2a2575H8bS_d4TxH",
					"type": "arrow"
				},
				{
					"id": "maVGMI1zh5XbbbxnQXXt_",
					"type": "arrow"
				},
				{
					"id": "YuGFG7czPr7ihAvgxdprE",
					"type": "arrow"
				}
			],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "S' -> S . \nS -> S . A\n----------- \nA -> . a",
			"rawText": "S' -> S . \nS -> S . A\n----------- \nA -> . a",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "S' -> S . \nS -> S . A\n----------- \nA -> . a",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 355,
			"versionNonce": 1723564134,
			"index": "b1X",
			"isDeleted": false,
			"id": "4F2Wvws0",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -391.90263154046715,
			"y": 3747.3883312877283,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 78.67996215820312,
			"height": 25,
			"seed": 2140878877,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "2VvNqkkoRspS0rnBJU2pz",
					"type": "arrow"
				}
			],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "S -> A .",
			"rawText": "S -> A .",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "S -> A .",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 219,
			"versionNonce": 352821498,
			"index": "b1x",
			"isDeleted": false,
			"id": "MjY2oT9r",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -390.392853363325,
			"y": 3841.245666850407,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 89.85997009277344,
			"height": 25,
			"seed": 823969811,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "ErY8bRrynSLjZzuA-Qj2j",
					"type": "arrow"
				},
				{
					"id": "YuGFG7czPr7ihAvgxdprE",
					"type": "arrow"
				}
			],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "A -> a . ",
			"rawText": "A -> a . ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "A -> a . ",
			"lineHeight": 1.25
		},
		{
			"type": "arrow",
			"version": 605,
			"versionNonce": 1501201318,
			"index": "b1y",
			"isDeleted": false,
			"id": "3uYPAZHgJkDJFXZXeykA-",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -570.4065109248219,
			"y": 3633.480467663191,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 165.29025128417777,
			"height": 0.9546250423190941,
			"seed": 1807524755,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "Fz2wQgjq"
				}
			],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "jPccM9hz",
				"focus": -0.8922963025958112,
				"gap": 9.591700906526626
			},
			"endBinding": {
				"elementId": "BkVSFbo2",
				"focus": 0.2439470733472514,
				"gap": 12.095037638737722
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					165.29025128417777,
					0.9546250423190941
				]
			]
		},
		{
			"type": "text",
			"version": 4,
			"versionNonce": 1948086714,
			"index": "b1z",
			"isDeleted": false,
			"id": "Fz2wQgjq",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 564.0746645369884,
			"y": 1328.185952091329,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.159988403320312,
			"height": 25,
			"seed": 1847731453,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "S",
			"rawText": "S",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "3uYPAZHgJkDJFXZXeykA-",
			"originalText": "S",
			"lineHeight": 1.25
		},
		{
			"type": "arrow",
			"version": 573,
			"versionNonce": 2079792870,
			"index": "b20",
			"isDeleted": false,
			"id": "2VvNqkkoRspS0rnBJU2pz",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -568.0337571032276,
			"y": 3704.7734440122276,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 166.46708687634413,
			"height": 56.03934639831459,
			"seed": 1197106909,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "s03Vh6bb"
				}
			],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "jPccM9hz",
				"focus": -0.06718418602425734,
				"gap": 11.964454728120927
			},
			"endBinding": {
				"elementId": "4F2Wvws0",
				"focus": -0.6767228399070226,
				"gap": 9.664038686416234
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					166.46708687634413,
					56.03934639831459
				]
			]
		},
		{
			"type": "text",
			"version": 4,
			"versionNonce": 968567418,
			"index": "b21",
			"isDeleted": false,
			"id": "s03Vh6bb",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 570.5105793433759,
			"y": 1412.2976732077118,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.1199951171875,
			"height": 25,
			"seed": 155015315,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "A",
			"rawText": "A",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "2VvNqkkoRspS0rnBJU2pz",
			"originalText": "A",
			"lineHeight": 1.25
		},
		{
			"type": "arrow",
			"version": 621,
			"versionNonce": 851333670,
			"index": "b22",
			"isDeleted": false,
			"id": "ErY8bRrynSLjZzuA-Qj2j",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -566.4229556904183,
			"y": 3752.381244697114,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 169.48283651789382,
			"height": 103.29058559647638,
			"seed": 802618365,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "Nk5LmxQA"
				}
			],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "jPccM9hz",
				"focus": 0.26057956607929944,
				"gap": 13.594951425778731
			},
			"endBinding": {
				"elementId": "MjY2oT9r",
				"focus": -0.8349237791352137,
				"gap": 6.54726580919953
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					169.48283651789382,
					103.29058559647638
				]
			]
		},
		{
			"type": "text",
			"version": 4,
			"versionNonce": 480496442,
			"index": "b23",
			"isDeleted": false,
			"id": "Nk5LmxQA",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 569.8065217966683,
			"y": 1490.0559343239192,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.339996337890625,
			"height": 25,
			"seed": 1171615795,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "a",
			"rawText": "a",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "ErY8bRrynSLjZzuA-Qj2j",
			"originalText": "a",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 136,
			"versionNonce": 1220353382,
			"index": "b24",
			"isDeleted": false,
			"id": "V9iY6Krj",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -108.53264592495043,
			"y": 3595.6915172791414,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 65.29994201660156,
			"height": 25,
			"seed": 1369968861,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "qa7Hw2a2575H8bS_d4TxH",
					"type": "arrow"
				}
			],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Accept",
			"rawText": "Accept",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Accept",
			"lineHeight": 1.25
		},
		{
			"type": "arrow",
			"version": 188,
			"versionNonce": 54154234,
			"index": "b25",
			"isDeleted": false,
			"id": "qa7Hw2a2575H8bS_d4TxH",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -278.87998134319844,
			"y": 3604.85248168359,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 162.32065318771117,
			"height": 1.7977708713310676,
			"seed": 770763581,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "qgaEzWDb"
				}
			],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "BkVSFbo2",
				"focus": -0.8209574387616609,
				"gap": 13.301290097184506
			},
			"endBinding": {
				"elementId": "V9iY6Krj",
				"focus": 0.4344181478003844,
				"gap": 8.026682230536835
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					162.32065318771117,
					-1.7977708713310676
				]
			]
		},
		{
			"type": "text",
			"version": 4,
			"versionNonce": 591429798,
			"index": "b26",
			"isDeleted": false,
			"id": "qgaEzWDb",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -203.31489339077257,
			"y": 3629.5164468172734,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16.05999755859375,
			"height": 25,
			"seed": 153138675,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "$",
			"rawText": "$",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "qa7Hw2a2575H8bS_d4TxH",
			"originalText": "$",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 120,
			"versionNonce": 260162746,
			"index": "b2L",
			"isDeleted": false,
			"id": "NPpSps6G",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -107.50118966793275,
			"y": 3647.794914624377,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 100.83995056152344,
			"height": 25,
			"seed": 1033459923,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [
				{
					"id": "maVGMI1zh5XbbbxnQXXt_",
					"type": "arrow"
				}
			],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "S -> SA . ",
			"rawText": "S -> SA . ",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "S -> SA . ",
			"lineHeight": 1.25
		},
		{
			"type": "arrow",
			"version": 310,
			"versionNonce": 1979022310,
			"index": "b2M",
			"isDeleted": false,
			"id": "maVGMI1zh5XbbbxnQXXt_",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -280.8792237179118,
			"y": 3666.3507610855263,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 167.78355114154567,
			"height": 2.678314119881179,
			"seed": 2025722355,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "NBv96Um6"
				}
			],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "BkVSFbo2",
				"focus": 0.39900696682707637,
				"gap": 11.302047722471116
			},
			"endBinding": {
				"elementId": "NPpSps6G",
				"focus": -0.18665212469256934,
				"gap": 5.594482908433406
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					167.78355114154567,
					-2.678314119881179
				]
			]
		},
		{
			"type": "text",
			"version": 4,
			"versionNonce": 723328378,
			"index": "b2N",
			"isDeleted": false,
			"id": "NBv96Um6",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -200.26162803892709,
			"y": 3698.8362498351994,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.1199951171875,
			"height": 25,
			"seed": 1276442973,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "A",
			"rawText": "A",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "maVGMI1zh5XbbbxnQXXt_",
			"originalText": "A",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 13,
			"versionNonce": 1994985254,
			"index": "b2i",
			"isDeleted": false,
			"id": "HalvZ0oz",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -695.5672017501731,
			"y": 3594.1877282078794,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 24.659988403320312,
			"height": 25,
			"seed": 101235645,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "I0",
			"rawText": "I0",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "I0",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 5,
			"versionNonce": 323968570,
			"index": "b2j",
			"isDeleted": false,
			"id": "uNVFn6lS",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -390.4414556543911,
			"y": 3573.06907240411,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 16.319992065429688,
			"height": 25,
			"seed": 583259485,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "I1",
			"rawText": "I1",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "I1",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 5,
			"versionNonce": 310917734,
			"index": "b2k",
			"isDeleted": false,
			"id": "TlEmJxu0",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -299.37320229987074,
			"y": 3752.640276201756,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 25.139984130859375,
			"height": 25,
			"seed": 587875091,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "I2",
			"rawText": "I2",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "I2",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 5,
			"versionNonce": 1694205690,
			"index": "b2l",
			"isDeleted": false,
			"id": "lftxevVO",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -363.5057750847442,
			"y": 3882.1880732272,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 24.519989013671875,
			"height": 25,
			"seed": 337100819,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "I3",
			"rawText": "I3",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "I3",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 36,
			"versionNonce": 530578854,
			"index": "b2n",
			"isDeleted": false,
			"id": "sK6gAtCG",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -84.60423882927671,
			"y": 3671.3873126976705,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 23.699981689453125,
			"height": 25,
			"seed": 1351210493,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "I4",
			"rawText": "I4",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "I4",
			"lineHeight": 1.25
		},
		{
			"type": "arrow",
			"version": 670,
			"versionNonce": 681875386,
			"index": "b3A",
			"isDeleted": false,
			"id": "YuGFG7czPr7ihAvgxdprE",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -278.5777234355436,
			"y": 3686.9811034252757,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 175.64132334803287,
			"height": 167.64445088247658,
			"seed": 331960806,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [
				{
					"type": "text",
					"id": "jRpzKYH9"
				}
			],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"startBinding": {
				"elementId": "BkVSFbo2",
				"focus": 0.1310276800022976,
				"gap": 13.603548004839354
			},
			"endBinding": {
				"elementId": "MjY2oT9r",
				"focus": 0.7440209811619327,
				"gap": 4.4083083721496905
			},
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": "arrow",
			"points": [
				[
					0,
					0
				],
				[
					158.09447188517458,
					74.68293864554153
				],
				[
					-17.546851462858285,
					167.64445088247658
				]
			]
		},
		{
			"type": "text",
			"version": 4,
			"versionNonce": 324884710,
			"index": "b3B",
			"isDeleted": false,
			"id": "jRpzKYH9",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -136.422435431581,
			"y": 3800.9088647663134,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.339996337890625,
			"height": 25,
			"seed": 1587156666,
			"groupIds": [
				"8dYZpZvBi6mqQTd1fI6Kc"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911792693,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "a",
			"rawText": "a",
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "YuGFG7czPr7ihAvgxdprE",
			"originalText": "a",
			"lineHeight": 1.25
		},
		{
			"type": "image",
			"version": 455,
			"versionNonce": 192750970,
			"index": "b3C8",
			"isDeleted": false,
			"id": "YbyHKJJgDaWr9v1DdQdTy",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1193.4044202452458,
			"y": 3625.530588214798,
			"strokeColor": "transparent",
			"backgroundColor": "transparent",
			"width": 396.4774526985413,
			"height": 139.056810132265,
			"seed": 955101798,
			"groupIds": [
				"FA4vEfDLS6ay-MTKKGYHl"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911784081,
			"link": null,
			"locked": false,
			"status": "pending",
			"fileId": "8c9922bc8ef58272539f6a9ee731c8b5f62d1093",
			"scale": [
				1,
				1
			]
		},
		{
			"type": "text",
			"version": 347,
			"versionNonce": 2054055482,
			"index": "b3CG",
			"isDeleted": false,
			"id": "IfBpUPrp",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -943.8317575006588,
			"y": 3617.619774964885,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 13.759994506835938,
			"height": 25,
			"seed": 1480477542,
			"groupIds": [
				"FA4vEfDLS6ay-MTKKGYHl"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911784081,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "0",
			"rawText": "0",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "0",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 319,
			"versionNonce": 586780410,
			"index": "b3CV",
			"isDeleted": false,
			"id": "DFpg6nzG",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -823.6077167299944,
			"y": 3617.166849698727,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 5.4199981689453125,
			"height": 25,
			"seed": 2123000314,
			"groupIds": [
				"FA4vEfDLS6ay-MTKKGYHl"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911784081,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "1",
			"rawText": "1",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "1",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 345,
			"versionNonce": 161587130,
			"index": "b3Cl",
			"isDeleted": false,
			"id": "HoxOALP8",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -974.6085816839786,
			"y": 3773.2824560729837,
			"strokeColor": "#1971c2",
			"backgroundColor": "transparent",
			"width": 14.239990234375,
			"height": 25,
			"seed": 1077225082,
			"groupIds": [
				"FA4vEfDLS6ay-MTKKGYHl"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911784081,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "2",
			"rawText": "2",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "2",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 363,
			"versionNonce": 713660538,
			"index": "b3D",
			"isDeleted": false,
			"id": "48HX4aeO",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -1126.7863264016555,
			"y": 3871.973086934571,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 269.60040283203125,
			"height": 73.77488588276213,
			"seed": 1773757414,
			"groupIds": [
				"FA4vEfDLS6ay-MTKKGYHl"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911784081,
			"link": null,
			"locked": false,
			"fontSize": 29.509954353104856,
			"fontFamily": 1,
			"text": "Follow(S) = {$, a}\nFollow(A) = {$, a}",
			"rawText": "Follow(S) = {$, a}\nFollow(A) = {$, a}",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Follow(S) = {$, a}\nFollow(A) = {$, a}",
			"lineHeight": 1.25
		},
		{
			"type": "freedraw",
			"version": 78,
			"versionNonce": 1976140922,
			"index": "b3e",
			"isDeleted": false,
			"id": "702ewkgUK1TcTfB8gus0s",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 47.009858513470135,
			"y": 3032.0359244224046,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 90.96094677250744,
			"height": 222.69657609486285,
			"seed": 1825471354,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911735736,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-3.2384108923470194,
					-0.7917933702251503
				],
				[
					-4.286179106291229,
					-1.1877208141509072
				],
				[
					-5.714987498556866,
					-1.6826301190581034
				],
				[
					-5.714987498556866,
					-1.8805323233946183
				],
				[
					-5.048259462934084,
					-1.9795141843760575
				],
				[
					-3.619451070668447,
					-2.0784960453574968
				],
				[
					-1.238226785478446,
					-2.0784960453574968
				],
				[
					5.524159821263538,
					-1.781550462413179
				],
				[
					9.810338927554767,
					-1.4846048794688613
				],
				[
					14.477435176914241,
					-0.9897570921880288
				],
				[
					24.097315532934772,
					0.6928730268705294
				],
				[
					28.574076246012964,
					1.9795141843765123
				],
				[
					36.09854320939803,
					5.839560692147643
				],
				[
					38.76545535188916,
					8.41296604241279
				],
				[
					40.765639458757505,
					11.58020104094021
				],
				[
					41.90851392321588,
					15.341327205356265
				],
				[
					42.38490642255738,
					19.696283018034592
				],
				[
					42.19432481577019,
					24.54614813562057
				],
				[
					40.19414070890184,
					35.82940359361601
				],
				[
					37.241417673856404,
					48.399423244370155
				],
				[
					35.812855352096676,
					54.733893241424994
				],
				[
					34.574505531365276,
					60.870399516516954
				],
				[
					33.33627874588683,
					71.95569125254951
				],
				[
					33.52686035267402,
					76.7065745091536
				],
				[
					34.28881767406392,
					80.8635665998695
				],
				[
					35.812855352096676,
					84.42672904232268
				],
				[
					38.003374995246304,
					87.29701845790532
				],
				[
					40.86086874452462,
					89.37551450326328
				],
				[
					48.19487713637545,
					91.0582061399482
				],
				[
					56.3860721353833,
					90.16736939111479
				],
				[
					60.386440349119994,
					89.17761229892676
				],
				[
					64.00589141978821,
					88.08887334575729
				],
				[
					69.72063284783917,
					86.10935916138078
				],
				[
					71.81616927572759,
					85.4164861345107
				],
				[
					73.34008391850739,
					85.02062020821131
				],
				[
					74.48308141821872,
					85.02062020821131
				],
				[
					75.1498094538415,
					85.71343171745502
				],
				[
					75.1498094538415,
					89.77144194718903
				],
				[
					74.00681195413017,
					97.39267613700304
				],
				[
					73.14962534697315,
					102.34146159794363
				],
				[
					72.48289731135037,
					108.0821019467362
				],
				[
					71.9113985614947,
					114.51555380477203
				],
				[
					71.43525213265912,
					128.76814205695882
				],
				[
					71.6255876689404,
					136.19135100718313
				],
				[
					72.1019801682819,
					143.61455995740744
				],
				[
					72.95904374018596,
					150.74082332468743
				],
				[
					74.00681195413017,
					157.57020262664946
				],
				[
					76.57849481085418,
					169.7442333158515
				],
				[
					79.34063623911265,
					179.74084761634094
				],
				[
					80.67409231035822,
					183.8978397070564
				],
				[
					81.81708981006955,
					187.46100214950957
				],
				[
					82.8647349887608,
					190.5293168046819
				],
				[
					84.5792312383278,
					195.1811566826782
				],
				[
					85.24595927395058,
					198.3483916812056
				],
				[
					85.05550070241634,
					199.6350943563384
				],
				[
					84.5792312383278,
					200.92179703147076
				],
				[
					83.6266923101507,
					202.30748156758455
				],
				[
					82.19800695313802,
					203.59412272509098
				],
				[
					77.91195088209975,
					206.365491797319
				],
				[
					75.05445713282143,
					207.75111481580643
				],
				[
					71.81616927572759,
					209.2357812129021
				],
				[
					68.3871767765936,
					210.72044760999734
				],
				[
					64.76784874117811,
					212.10613214611112
				],
				[
					57.6244219561147,
					214.87743970071278
				],
				[
					54.290781778000564,
					216.16414237584559
				],
				[
					48.48056499367681,
					218.5395840041474
				],
				[
					46.19469302950711,
					219.52934109633588
				],
				[
					44.28973820840588,
					220.22215260557914
				],
				[
					42.86105285139297,
					220.61808004950535
				],
				[
					41.33713820861317,
					220.61808004950535
				],
				[
					41.33713820861317,
					220.12323226222452
				],
				[
					41.813407672701715,
					219.43035923535444
				],
				[
					42.67059427985873,
					218.44060214316596
				],
				[
					43.90869803008445,
					217.25288132901505
				],
				[
					45.527964993884325,
					215.96617865388225
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.0117647061124444,
				0.2666666805744171,
				0.37254902720451355,
				0.5176470875740051,
				0.5568627715110779,
				0.5843137502670288,
				0.6039215922355652,
				0.6117647290229797,
				0.6235294342041016,
				0.6274510025978088,
				0.6274510025978088,
				0.6313725709915161,
				0.6313725709915161,
				0.6313725709915161,
				0.6352941393852234,
				0.6352941393852234,
				0.6392157077789307,
				0.6470588445663452,
				0.6549019813537598,
				0.6745098233222961,
				0.6980392336845398,
				0.7058823704719543,
				0.7176470756530762,
				0.7254902124404907,
				0.729411780834198,
				0.7333333492279053,
				0.7333333492279053,
				0.7372549176216125,
				0.7372549176216125,
				0.7333333492279053,
				0.7333333492279053,
				0.729411780834198,
				0.729411780834198,
				0.729411780834198,
				0.729411780834198,
				0.729411780834198,
				0.7333333492279053,
				0.7372549176216125,
				0.7490196228027344,
				0.7686274647712708,
				0.7764706015586853,
				0.7803921699523926,
				0.7882353067398071,
				0.7960784435272217,
				0.7960784435272217,
				0.7960784435272217,
				0.800000011920929,
				0.800000011920929,
				0.800000011920929,
				0.800000011920929,
				0.800000011920929,
				0.800000011920929,
				0.800000011920929,
				0.8039215803146362,
				0.8156862854957581,
				0.8235294222831726,
				0.8313725590705872,
				0.8392156958580017,
				0.8470588326454163,
				0.8627451062202454,
				0.8666666746139526,
				0.8705882430076599,
				0.8745098114013672,
				0.8784313797950745,
				0.8784313797950745,
				0.8745098114013672,
				0.8509804010391235,
				0.8274509906768799,
				0.7843137383460999,
				0.7215686440467834,
				0.4941176474094391,
				0.364705890417099,
				0.239215686917305,
				0.12941177189350128,
				0.03921568766236305,
				0
			]
		},
		{
			"type": "text",
			"version": 28,
			"versionNonce": 448283430,
			"index": "b3f",
			"isDeleted": false,
			"id": "LxOhZHB6",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 232.64618634441445,
			"y": 3107.950705561333,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 229.67977905273438,
			"height": 25,
			"seed": 526426982,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911744203,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "predictive parsing table",
			"rawText": "predictive parsing table",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "predictive parsing table",
			"lineHeight": 1.25
		},
		{
			"type": "line",
			"version": 1899,
			"versionNonce": 1303228518,
			"index": "b3f1",
			"isDeleted": false,
			"id": "TUCg7K65-hPBZQ_KnykMY",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -653.4773045081716,
			"y": 4046.8970152813554,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 793.0039562923896,
			"height": 2.219179467027516,
			"seed": 963225629,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					793.0039562923896,
					2.219179467027516
				]
			]
		},
		{
			"type": "line",
			"version": 1133,
			"versionNonce": 1905291514,
			"index": "b3f2",
			"isDeleted": false,
			"id": "_5a1J2bf5E0KMlZoOR6ww",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -519.5961473246548,
			"y": 3990.187067552571,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 1.1368683772161603e-13,
			"height": 414.3915956633893,
			"seed": 1771609213,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					-1.1368683772161603e-13,
					414.3915956633893
				]
			]
		},
		{
			"type": "text",
			"version": 650,
			"versionNonce": 44479398,
			"index": "b3f4",
			"isDeleted": false,
			"id": "urKuEnLa",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -314.20089647297254,
			"y": 4002.1842671806216,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 46.23994445800781,
			"height": 25,
			"seed": 2117034301,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "input",
			"rawText": "input",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "input",
			"lineHeight": 1.25
		},
		{
			"type": "line",
			"version": 2014,
			"versionNonce": 1728856506,
			"index": "b3f6",
			"isDeleted": false,
			"id": "prBXhki1ofPv3bBVWWuaO",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -651.1076005557413,
			"y": 4106.733441116333,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 789.634578982537,
			"height": 2.0504879408944134,
			"seed": 998912413,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					789.634578982537,
					2.0504879408944134
				]
			]
		},
		{
			"type": "line",
			"version": 1940,
			"versionNonce": 270356198,
			"index": "b3f8",
			"isDeleted": false,
			"id": "TTGbb9IV__3yO0BDhyvBV",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -654.7090637903423,
			"y": 4162.33212785179,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 789.634578982537,
			"height": 2.0504879408944134,
			"seed": 971765245,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					789.634578982537,
					2.0504879408944134
				]
			]
		},
		{
			"type": "line",
			"version": 1964,
			"versionNonce": 105904762,
			"index": "b3fA",
			"isDeleted": false,
			"id": "oRKldq1CzWOngNWjOPGk4",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -655.3852373137495,
			"y": 4218.963981398919,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 789.634578982537,
			"height": 2.0504879408944134,
			"seed": 609627741,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					789.634578982537,
					2.0504879408944134
				]
			]
		},
		{
			"type": "line",
			"version": 1276,
			"versionNonce": 1117684262,
			"index": "b3fC",
			"isDeleted": false,
			"id": "PSvkaVYBEzkgI7kPqdXtP",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -658.1762514316429,
			"y": 4284.836192664287,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 789.634578982537,
			"height": 2.0504879408944134,
			"seed": 1234852541,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					789.634578982537,
					2.0504879408944134
				]
			]
		},
		{
			"type": "line",
			"version": 1075,
			"versionNonce": 505322298,
			"index": "b3fE",
			"isDeleted": false,
			"id": "ig1bn20SBf2OYpOJwgS1O",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -363.67163832010874,
			"y": 4042.5850880237394,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.684341886080802e-14,
			"height": 358.2337848018293,
			"seed": 150770749,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					-5.684341886080802e-14,
					358.2337848018293
				]
			]
		},
		{
			"type": "line",
			"version": 1481,
			"versionNonce": 1293372774,
			"index": "b3fG",
			"isDeleted": false,
			"id": "3Keu1qRXylJ8C_QxOnN--",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -203.78248212947938,
			"y": 4051.0814317218114,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.263256414560601e-14,
			"height": 358.0071870431348,
			"seed": 1128818941,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					-4.263256414560601e-14,
					358.0071870431348
				]
			]
		},
		{
			"type": "text",
			"version": 489,
			"versionNonce": 752559098,
			"index": "b3fH",
			"isDeleted": false,
			"id": "0VjkQ4HA",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -453.85002859332735,
			"y": 4073.7456324310742,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.339996337890625,
			"height": 25,
			"seed": 1336688989,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "a",
			"rawText": "a",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "a",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 838,
			"versionNonce": 2094313638,
			"index": "b3fI",
			"isDeleted": false,
			"id": "BPORJAuw",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -295.2505726675008,
			"y": 4084.2900302184407,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 16.05999755859375,
			"height": 25,
			"seed": 663178781,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "$",
			"rawText": "$",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "$",
			"lineHeight": 1.25
		},
		{
			"type": "line",
			"version": 1384,
			"versionNonce": 1820890298,
			"index": "b3fK",
			"isDeleted": false,
			"id": "oX4lgzPPtgJK6N1f6GDwc",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -654.5801356368479,
			"y": 4345.691298900706,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 789.634578982537,
			"height": 2.0504879408944134,
			"seed": 614038717,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					789.634578982537,
					2.0504879408944134
				]
			]
		},
		{
			"type": "line",
			"version": 1408,
			"versionNonce": 1837345766,
			"index": "b3fM",
			"isDeleted": false,
			"id": "rkSQ3vCeEoVYjVtCbcuWk",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -655.2563091602551,
			"y": 4402.323152447835,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 789.634578982537,
			"height": 2.0504879408944134,
			"seed": 1428479261,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					789.634578982537,
					2.0504879408944134
				]
			]
		},
		{
			"type": "line",
			"version": 1713,
			"versionNonce": 1590291834,
			"index": "b3fO",
			"isDeleted": false,
			"id": "1PcjKumDAbTyiwiU5Zw66",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -37.859547727985614,
			"y": 4047.130612796243,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.263256414560601e-14,
			"height": 358.0071870431348,
			"seed": 1643236538,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					-4.263256414560601e-14,
					358.0071870431348
				]
			]
		},
		{
			"type": "line",
			"version": 1656,
			"versionNonce": 1026637606,
			"index": "b3fQ",
			"isDeleted": false,
			"id": "Fp6beKI-p8VbNZCsnMC3u",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 135.51640156765757,
			"y": 4051.7832650497407,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 4.263256414560601e-14,
			"height": 358.0071870431348,
			"seed": 793871846,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": {
				"type": 2
			},
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"startBinding": null,
			"endBinding": null,
			"lastCommittedPoint": null,
			"startArrowhead": null,
			"endArrowhead": null,
			"points": [
				[
					0,
					0
				],
				[
					-4.263256414560601e-14,
					358.0071870431348
				]
			]
		},
		{
			"type": "text",
			"version": 416,
			"versionNonce": 1491217978,
			"index": "b3fS",
			"isDeleted": false,
			"id": "fSV3beL4",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -127.85889585063353,
			"y": 4080.967743484476,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.159988403320312,
			"height": 25,
			"seed": 2019463718,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "S",
			"rawText": "S",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "S",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 422,
			"versionNonce": 1078618726,
			"index": "b3fU",
			"isDeleted": false,
			"id": "kgJOVYOt",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 35.016792424654795,
			"y": 4080.264803867706,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.1199951171875,
			"height": 25,
			"seed": 563204838,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "A",
			"rawText": "A",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "A",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 5,
			"versionNonce": 263476986,
			"index": "b3fV",
			"isDeleted": false,
			"id": "GLF9RjvI",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -598.9448624939257,
			"y": 4126.65659252859,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.759994506835938,
			"height": 25,
			"seed": 408649190,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "0",
			"rawText": "0",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "0",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 5,
			"versionNonce": 899427750,
			"index": "b3fW",
			"isDeleted": false,
			"id": "qX8ZFs73",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -598.9448624939257,
			"y": 4181.635628699242,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.4199981689453125,
			"height": 25,
			"seed": 2078590246,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "1",
			"rawText": "1",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "1",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 5,
			"versionNonce": 600008634,
			"index": "b3fX",
			"isDeleted": false,
			"id": "EdDlhQOx",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -596.6540693201487,
			"y": 4241.19625121745,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.239990234375,
			"height": 25,
			"seed": 1899090810,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "2",
			"rawText": "2",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "2",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 5,
			"versionNonce": 2052294886,
			"index": "b3fZ",
			"isDeleted": false,
			"id": "BPkUGq8O",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -602.3810522545916,
			"y": 4314.50163277832,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 13.6199951171875,
			"height": 25,
			"seed": 1367866214,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "3",
			"rawText": "3",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "3",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 5,
			"versionNonce": 758276218,
			"index": "b3fb",
			"isDeleted": false,
			"id": "7qtllvuc",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -594.3632761463714,
			"y": 4374.062255296526,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.79998779296875,
			"height": 25,
			"seed": 859304166,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "4",
			"rawText": "4",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "4",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 425,
			"versionNonce": 1040022566,
			"index": "b3fd",
			"isDeleted": false,
			"id": "MpF8ftuS",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -124.14350238291354,
			"y": 4131.790840450167,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 5.4199981689453125,
			"height": 25,
			"seed": 259064614,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "1",
			"rawText": "1",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "1",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 519,
			"versionNonce": 1204044090,
			"index": "b3ff",
			"isDeleted": false,
			"id": "Zs8GKmY8",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 38.68468731637563,
			"y": 4128.510158415776,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.239990234375,
			"height": 25,
			"seed": 1186510202,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "2",
			"rawText": "2",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "2",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 104,
			"versionNonce": 914818918,
			"index": "b3fh",
			"isDeleted": false,
			"id": "OzFhhoHP",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -459.8004455919681,
			"y": 4127.9505593679205,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 24.47998046875,
			"height": 25,
			"seed": 545006118,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "s3",
			"rawText": "s3",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "s3",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 552,
			"versionNonce": 517736954,
			"index": "b3fj",
			"isDeleted": false,
			"id": "TACY0qzJ",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -315.57562831329847,
			"y": 4184.956013478969,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 65.29994201660156,
			"height": 25,
			"seed": 3916326,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "Accept",
			"rawText": "Accept",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "Accept",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 354,
			"versionNonce": 1413294758,
			"index": "b3fl",
			"isDeleted": false,
			"id": "YyFMc7D4",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 47.21263089613444,
			"y": 4196.539746240437,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 12.79998779296875,
			"height": 25,
			"seed": 648954234,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "4",
			"rawText": "4",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "4",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 6,
			"versionNonce": 2038217402,
			"index": "b3fm",
			"isDeleted": false,
			"id": "qndYqdnO",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -457.73723688411155,
			"y": 4184.525595950058,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 24.47998046875,
			"height": 25,
			"seed": 2095822906,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "s3",
			"rawText": "s3",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "s3",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 315,
			"versionNonce": 1976362470,
			"index": "b3fn",
			"isDeleted": false,
			"id": "s796J56R",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -452.2576932458943,
			"y": 4240.163035380177,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.019989013671875,
			"height": 25,
			"seed": 1913735546,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "r1",
			"rawText": "r1",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "r1",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 832,
			"versionNonce": 1179210618,
			"index": "b3fp",
			"isDeleted": false,
			"id": "tXuF8WGh",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -285.97225315779167,
			"y": 4239.210701321044,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 14.019989013671875,
			"height": 25,
			"seed": 1719223014,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "r1",
			"rawText": "r1",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "r1",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 322,
			"versionNonce": 474167590,
			"index": "b3fr",
			"isDeleted": false,
			"id": "8zPOBmsj",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -454.30198783793924,
			"y": 4310.47518693296,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 22.839981079101562,
			"height": 25,
			"seed": 309334502,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "r2",
			"rawText": "r2",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "r2",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 438,
			"versionNonce": 663016506,
			"index": "b3ft",
			"isDeleted": false,
			"id": "dOx1rU4X",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -287.5871746333995,
			"y": 4308.737876082274,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 22.839981079101562,
			"height": 25,
			"seed": 717483814,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "r2",
			"rawText": "r2",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "r2",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 1078,
			"versionNonce": 520954982,
			"index": "b3fv",
			"isDeleted": false,
			"id": "swFv2x3w",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -453.29122096782896,
			"y": 4366.974384648686,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 22.3599853515625,
			"height": 25,
			"seed": 544568422,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "r0",
			"rawText": "r0",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "r0",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 1066,
			"versionNonce": 2131901690,
			"index": "b3fx",
			"isDeleted": false,
			"id": "IeEIOZDR",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -290.0037529827446,
			"y": 4370.18557872422,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 22.3599853515625,
			"height": 25,
			"seed": 1953252966,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "r0",
			"rawText": "r0",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "r0",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 165,
			"versionNonce": 1610065830,
			"index": "b3fz",
			"isDeleted": false,
			"id": "PiIl88wi",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": -622.0543762698545,
			"y": 4004.263957038287,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"width": 57.73994445800781,
			"height": 25,
			"seed": 951524730,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788674,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "state",
			"rawText": "state",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "state",
			"lineHeight": 1.25
		},
		{
			"type": "text",
			"version": 57,
			"versionNonce": 1459963174,
			"index": "b3g",
			"isDeleted": false,
			"id": "sNJmXRnC",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 267.2198306290102,
			"y": 4195.159469290263,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 195.57984924316406,
			"height": 25,
			"seed": 1057430650,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788673,
			"link": null,
			"locked": false,
			"fontSize": 20,
			"fontFamily": 1,
			"text": "SLR(1) parsing table",
			"rawText": "SLR(1) parsing table",
			"textAlign": "left",
			"verticalAlign": "top",
			"containerId": null,
			"originalText": "SLR(1) parsing table",
			"lineHeight": 1.25
		},
		{
			"type": "freedraw",
			"version": 158,
			"versionNonce": 2058979386,
			"index": "b3h",
			"isDeleted": false,
			"id": "BgaYFVD6im0Qy08t6IXrS",
			"fillStyle": "solid",
			"strokeWidth": 0.5,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"angle": 0,
			"x": 164.4387640723512,
			"y": 4068.9421556146567,
			"strokeColor": "#f08c00",
			"backgroundColor": "transparent",
			"width": 81.24559106021388,
			"height": 328.60120013525966,
			"seed": 531579642,
			"groupIds": [
				"t7DPzLTs-8x7e9eHQqRow"
			],
			"frameId": null,
			"roundness": null,
			"boundElements": [],
			"updated": 1721911788673,
			"link": null,
			"locked": false,
			"points": [
				[
					0,
					0
				],
				[
					-1.714496249567219,
					0.2969455829443177
				],
				[
					-2.285871964169928,
					0.3959889615521206
				],
				[
					-2.6669121424913556,
					0.49497082253355984
				],
				[
					-2.6669121424913556,
					1.0888004707962864
				],
				[
					-2.0955364278886464,
					1.5836482580766642
				],
				[
					-1.0477682139444369,
					2.27645976732083
				],
				[
					0.476146428835591,
					3.068314655172344
				],
				[
					2.3812242851897736,
					3.9590898863789334
				],
				[
					7.143426785063411,
					5.8396222097740065
				],
				[
					9.905691248574612,
					6.73045895860696
				],
				[
					12.858291248367323,
					7.621111154560822
				],
				[
					16.001472854946996,
					8.51194790339423
				],
				[
					19.335113033060907,
					9.402784652227183
				],
				[
					22.763982496942162,
					10.293559883433772
				],
				[
					29.90753231725853,
					12.471037789773163
				],
				[
					33.43175410215963,
					13.955765704494752
				],
				[
					36.76539428027377,
					15.737193131655204
				],
				[
					39.81322356583337,
					17.81575069463952
				],
				[
					42.4801357083245,
					20.389156044904666
				],
				[
					44.86123695826154,
					23.25944546048777
				],
				[
					46.86142106512989,
					26.525662319996627
				],
				[
					48.48068802892976,
					30.187806623430788
				],
				[
					50.6714537425853,
					38.303827082898806
				],
				[
					51.14760017142089,
					42.75770323893312
				],
				[
					51.33818177820808,
					47.409666152182126
				],
				[
					51.33818177820808,
					52.160549408786665
				],
				[
					51.14760017142089,
					57.109273352100445
				],
				[
					50.76655999309946,
					62.15716370927521
				],
				[
					50.29041356426387,
					67.20493103119816
				],
				[
					49.052186778785426,
					77.20154533168761
				],
				[
					48.48068802892976,
					81.95230555303851
				],
				[
					48.19487713637545,
					86.40630474432464
				],
				[
					48.099647850608335,
					90.46425345643229
				],
				[
					48.19487713637545,
					94.02747741651228
				],
				[
					48.48068802892976,
					97.09573055405826
				],
				[
					48.76637588623112,
					99.66913590432296
				],
				[
					49.4331039218539,
					103.62804123782325
				],
				[
					49.81414410017533,
					105.11270763491802
				],
				[
					50.29041356426387,
					106.3004899666962
				],
				[
					50.76655999309946,
					107.29018554125787
				],
				[
					51.81432820704367,
					108.77485193835355
				],
				[
					52.385826956899336,
					109.36874310424218
				],
				[
					53.81451231391202,
					110.55652543601946
				],
				[
					54.576592670554874,
					111.15041660190809
				],
				[
					55.43365624245894,
					111.744184732544
				],
				[
					56.29096588486891,
					112.43699624178817
				],
				[
					57.243504813046,
					113.12980775103142
				],
				[
					58.195920705970366,
					113.82274229552831
				],
				[
					59.1483365988945,
					114.6144741481271
				],
				[
					61.24387302678292,
					116.09914054522278
				],
				[
					62.291518205474176,
					116.79195205446604
				],
				[
					63.24405713365127,
					117.48488659896293
				],
				[
					64.1964730265754,
					118.17769810820619
				],
				[
					65.1490119547525,
					118.87050961745035
				],
				[
					66.95861445483365,
					120.0581689139749
				],
				[
					68.95879856170222,
					121.14690786714482
				],
				[
					69.91133748987932,
					121.6417556544252
				],
				[
					71.53048141842623,
					122.33469019892209
				],
				[
					72.19720945404902,
					122.6315742642405
				],
				[
					72.8639374896718,
					122.82953798620338
				],
				[
					73.43543623952746,
					123.02750170816626
				],
				[
					74.38797516770455,
					123.42342915209201
				],
				[
					74.76889231077303,
					123.62126983880216
				],
				[
					75.14993248909445,
					123.81935659601777
				],
				[
					75.43562034639581,
					124.01732031798065
				],
				[
					75.81666052471724,
					124.21528403994353
				],
				[
					76.29280695355283,
					124.31420438329815
				],
				[
					77.24522284647696,
					124.7101318272239
				],
				[
					78.00718016786686,
					125.10593623589693
				],
				[
					78.29299106042117,
					125.30389995785981
				],
				[
					78.48357266720836,
					125.40294333646807
				],
				[
					78.57867891772253,
					125.60090705843095
				],
				[
					78.57867891772253,
					125.7987477451411
				],
				[
					78.10253248888694,
					126.88760973356375
				],
				[
					77.1501165959628,
					129.06508763990269
				],
				[
					76.48338856034002,
					130.54975403699837
				],
				[
					75.9117667752314,
					132.43022484276707
				],
				[
					75.24503873960862,
					134.607702749106
				],
				[
					74.57831070398584,
					137.08206472076245
				],
				[
					73.91158266836305,
					139.85355682824365
				],
				[
					72.48302034660333,
					146.2868241334004
				],
				[
					71.14956427535776,
					153.512192396915
				],
				[
					70.57794249024914,
					157.1743367003496
				],
				[
					70.10179606141355,
					160.83648100378423
				],
				[
					69.625526597325,
					164.3995819286115
				],
				[
					69.3397157047707,
					167.96268285343785
				],
				[
					68.76833999016799,
					174.79200063777307
				],
				[
					68.4826521328664,
					178.05834053253557
				],
				[
					68.1968412403121,
					181.22551401343617
				],
				[
					67.72057177622355,
					187.2630999451726
				],
				[
					67.4348839189222,
					190.03446901740108
				],
				[
					67.14919606162084,
					192.7067947110213
				],
				[
					66.86338516906653,
					195.280200061286
				],
				[
					66.10130481242368,
					200.2290470398534
				],
				[
					65.7203876693552,
					202.70340901151076
				],
				[
					65.24424124051961,
					205.27681436177545
				],
				[
					64.76784874117811,
					207.85009667678742
				],
				[
					64.29170231234252,
					210.6214657490159
				],
				[
					63.81555588350693,
					213.4917551645981
				],
				[
					63.24405713365127,
					216.5601313373977
				],
				[
					62.100936598686985,
					223.0924420211618
				],
				[
					61.05329141999573,
					230.11984656271352
				],
				[
					60.6722512416743,
					233.68294748753988
				],
				[
					60.29133409860583,
					237.24617144761987
				],
				[
					59.91041695553736,
					240.80927237244623
				],
				[
					59.52937677721593,
					244.27345295391797
				],
				[
					58.67206713480596,
					251.1027707382541
				],
				[
					57.6244219561147,
					257.73424783587916
				],
				[
					57.05292320625904,
					260.90142131678067
				],
				[
					56.48142445640315,
					263.96967445432665
				],
				[
					55.91004874180044,
					267.03792759187263
				],
				[
					55.338549991944774,
					270.00713735081035
				],
				[
					54.290781778000564,
					275.7478392172293
				],
				[
					53.7192830281449,
					278.6181286328124
				],
				[
					53.24313659930931,
					281.38949770503996
				],
				[
					52.671637849453646,
					283.96290305530556
				],
				[
					52.195245350112145,
					286.437265026962
				],
				[
					51.623869635509436,
					288.71366327665646
				],
				[
					50.957141599886654,
					290.7922208396408
				],
				[
					49.62368552864109,
					294.4543651430754
				],
				[
					48.861605171998235,
					296.13699526213395
				],
				[
					48.099647850608335,
					297.72058200258425
				],
				[
					47.33781356447139,
					299.30416874303455
				],
				[
					46.480503922061416,
					300.88775548348576
				],
				[
					45.527964993884325,
					302.57050863779705
				],
				[
					43.43267463650159,
					306.1336095626234
				],
				[
					41.14667963707893,
					309.89467420941264
				],
				[
					40.00380517262056,
					311.7752680504341
				],
				[
					38.86068463765628,
					313.55669547759453
				],
				[
					37.81303945896502,
					315.33836897526135
				],
				[
					36.76539428027377,
					316.92195571571165
				],
				[
					35.812855352096676,
					318.4066221128073
				],
				[
					34.9555457096867,
					319.6933247879392
				],
				[
					33.24117249537244,
					321.77188235092353
				],
				[
					32.47921517398254,
					322.66253454687694
				],
				[
					31.621905531572565,
					323.45438943472936
				],
				[
					30.7648419596685,
					324.2462443225809
				],
				[
					29.81230303149141,
					324.93905583182504
				],
				[
					28.764657852800156,
					325.53282396246004
				],
				[
					26.383310532357427,
					326.6216859508827
				],
				[
					25.049854461111863,
					327.0174903595557
				],
				[
					23.7163983898663,
					327.4135408387342
				],
				[
					22.382942318620735,
					327.7103018687999
				],
				[
					19.811382497149452,
					328.3041930346885
				],
				[
					18.573155711671006,
					328.5021567566514
				],
				[
					17.43015821195968,
					328.60120013525966
				],
				[
					15.334744819324214,
					328.4032364132968
				],
				[
					14.76324606946855,
					328.007308969371
				],
				[
					14.572787497934314,
					327.4135408387342
				],
				[
					14.953827676255742,
					326.7206062942382
				],
				[
					15.810891248159805,
					326.2256354717042
				],
				[
					17.14434731940537,
					325.8298310630312
				],
				[
					19.049302140506597,
					325.6318673410683
				],
				[
					21.621108032483562,
					325.8298310630312
				]
			],
			"lastCommittedPoint": null,
			"simulatePressure": false,
			"pressures": [
				0.01568627543747425,
				0.30588236451148987,
				0.42352941632270813,
				0.5254902243614197,
				0.6470588445663452,
				0.6784313917160034,
				0.7019608020782471,
				0.7176470756530762,
				0.729411780834198,
				0.7450980544090271,
				0.7490196228027344,
				0.7529411911964417,
				0.7568627595901489,
				0.7568627595901489,
				0.7568627595901489,
				0.7607843279838562,
				0.7607843279838562,
				0.7607843279838562,
				0.7607843279838562,
				0.7607843279838562,
				0.7607843279838562,
				0.7607843279838562,
				0.7647058963775635,
				0.7647058963775635,
				0.7686274647712708,
				0.7686274647712708,
				0.772549033164978,
				0.7764706015586853,
				0.7764706015586853,
				0.7803921699523926,
				0.7843137383460999,
				0.7882353067398071,
				0.7882353067398071,
				0.7882353067398071,
				0.7882353067398071,
				0.7843137383460999,
				0.7843137383460999,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7843137383460999,
				0.7843137383460999,
				0.7843137383460999,
				0.7843137383460999,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7803921699523926,
				0.7843137383460999,
				0.7882353067398071,
				0.7921568751335144,
				0.7960784435272217,
				0.800000011920929,
				0.8039215803146362,
				0.8078431487083435,
				0.8156862854957581,
				0.8196078538894653,
				0.8235294222831726,
				0.8274509906768799,
				0.8274509906768799,
				0.8274509906768799,
				0.8274509906768799,
				0.8274509906768799,
				0.8274509906768799,
				0.8274509906768799,
				0.8274509906768799,
				0.8313725590705872,
				0.8313725590705872,
				0.8313725590705872,
				0.8313725590705872,
				0.8313725590705872,
				0.8313725590705872,
				0.8313725590705872,
				0.8313725590705872,
				0.8313725590705872,
				0.8313725590705872,
				0.8352941274642944,
				0.8352941274642944,
				0.8352941274642944,
				0.8352941274642944,
				0.8352941274642944,
				0.8392156958580017,
				0.8392156958580017,
				0.8392156958580017,
				0.8392156958580017,
				0.8392156958580017,
				0.843137264251709,
				0.843137264251709,
				0.843137264251709,
				0.843137264251709,
				0.843137264251709,
				0.843137264251709,
				0.8470588326454163,
				0.8470588326454163,
				0.8470588326454163,
				0.8470588326454163,
				0.8509804010391235,
				0.8509804010391235,
				0.8509804010391235,
				0.8549019694328308,
				0.8549019694328308,
				0.8588235378265381,
				0.8588235378265381,
				0.8627451062202454,
				0.8627451062202454,
				0.8627451062202454,
				0.8666666746139526,
				0.8666666746139526,
				0.8705882430076599,
				0.8705882430076599,
				0.8745098114013672,
				0.8745098114013672,
				0.8745098114013672,
				0.8745098114013672,
				0.8745098114013672,
				0.8745098114013672,
				0.8745098114013672,
				0.8745098114013672,
				0.8666666746139526,
				0.8549019694328308,
				0.8352941274642944,
				0.7333333492279053,
				0.6235294342041016,
				0.49803921580314636,
				0.3686274588108063,
				0.239215686917305,
				0.125490203499794,
				0.03921568766236305,
				0
			]
		}
	],
	"appState": {
		"theme": "light",
		"viewBackgroundColor": "#ffffff",
		"currentItemStrokeColor": "#f08c00",
		"currentItemBackgroundColor": "transparent",
		"currentItemFillStyle": "solid",
		"currentItemStrokeWidth": 0.5,
		"currentItemStrokeStyle": "solid",
		"currentItemRoughness": 1,
		"currentItemOpacity": 100,
		"currentItemFontFamily": 1,
		"currentItemFontSize": 20,
		"currentItemTextAlign": "left",
		"currentItemStartArrowhead": null,
		"currentItemEndArrowhead": "arrow",
		"scrollX": 1019.9016703904781,
		"scrollY": -2571.6608923587446,
		"zoom": {
			"value": 0.8717630949616432
		},
		"currentItemRoundness": "round",
		"gridSize": null,
		"gridColor": {
			"Bold": "#C9C9C9FF",
			"Regular": "#EDEDEDFF"
		},
		"currentStrokeOptions": null,
		"previousGridSize": null,
		"frameRendering": {
			"enabled": true,
			"clip": true,
			"name": true,
			"outline": true
		},
		"objectsSnapModeEnabled": false
	},
	"files": {}
}
```
%%
perfor.ma
=========

Node based network for sharing live data generated by human will.

<b>Dependencies</b>
<br />Node.js
<br />Socket.IO

<b>Role</b>
<p>
PERFOR.MA is a live performance tool. 
It allow you to share control data. 
</p>
<b>Work</b>
Each player diffuse on his channel. 
Data are structured as js object key : value
Keys are controler's name you update
Values are controller's position you update. [0-127]
Each time you update a value, you send on your channel an event contains an object like this one : 
<code>
	{
		username : {
			instrumentName : {
				key : value,
				date : timestamp
			}
		}
	}
</code>
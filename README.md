# ZENITH
ZENITH Protocol

Fixed the function used in the <a href="https://etherscan.io/token/0xcd0a53685b594a543181e6203433766648a8cd43" target="_blank">ZerroXBToken</a> contract <br>
( <i>function transfer(address _to, uint _value, string _message)</i> )<br>
to a new function: <br>
<i>// Transfer token with data and signature<br>
function transferAndData(address _to, uint _value, string _data)</i><br>

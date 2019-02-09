# ZENITH
ZENITH Protocol

Fixed the function used in the <a href="https://etherscan.io/token/0xcd0a53685b594a543181e6203433766648a8cd43" target="_blank">ZerroXBToken</a> contract <br>
( <i>function transfer(address _to, uint _value, string _message)</i> )<br>
to a new function: <br>

  Smart Contract 1 | zenith.sol :<br>
  https://etherscan.io/address/0xaa001c4cc0f1d15b11ce5baf410aa93b9ef96ecc<br>
<i>// Transfer token with data and signature<br>
function transferAndData(address _to, uint _value, string _data)</i><br>

Incorporates a new feature:<br>
<i>// Transfer any ERC token with data and signature<br>
function transferTokenData(address token, address _to, uint _value, string _data)</i><br>
  
  Smart Contract 2 | ZenithProtocol.sol :<br>
  https://etherscan.io/address/0x8C1ec84943CF6D70E2C92Ec81f1cbC320D5Cd2a8<br>
<i>// Transfer any ERC token with data and signature / or multi transfer with data and signature<br> 
//remember to call Token(address).approve(this, amount) or this contract will not be able to do the transfer on your behalf.<br>
function TransferTokenData(address _token, address[] addresses, uint amount, string _data) public</i><br>

<i>// Transfer Ether with data and signature / or multi transfer with data and signature <br>
function SendEthData(address[] addresses, string _data) public payable </i><br><br>
  
  https://zenith.0xbt.net

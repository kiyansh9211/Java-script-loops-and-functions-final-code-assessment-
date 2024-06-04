# Java-script-loops-and-functions-final-code-assessment-
(Metacrafters course)

const NFTs = []
function mintNFT (_name, _eyeColor, _shirtType, _bling) {
  const NFT = {
    "name": _name,
    "eyeColor": _eyeColor,
    "shirtType": _shirtType,
    "bling": _bling,
  }
  NFTs.push(NFT);
  console.log("Minted: " + _name);
}

function listNFTs () {
for(let i = 0; i < NFTs.length; i++) {
  console.log("\nID: \t\t" +(i+1))
  console.log("Name: \t\t" + NFTs[i].name);
  console.log("Eyecolor: \t" + NFTs[i].eyeColor);
  console.log("Shirt Type: " + NFTs[i].shirtType);
  console.log("Bling: \t\t" + NFTs[i].bling);
}
}

function getTotalSupply() {
console.log(NFTs.length);
}

mintNFT("Kiyansh", "Black", "White Tshirt", "Gold Ring");
mintNFT("Akshat", "Black", "Hoodie", "Silver chain");
mintNFT("Om", "Brown", "Black Shirt", "Gold Earing");
mintNFT("Ashu", "Blue", "Black Tshirt", "Gold Chain");
listNFTs();
getTotalSupply();

<h1>CENG-3550 ERC20 Tokeni ile Token oluşturma </h1>

ERC20, Ethereum’un ağında tokenları yayınlamak için belirli kuralları tanımlayan bir protokol standartıdır. Projenin amacı bu kurallara uyarak bir token oluşturmak ve bazı transactionlar yapmaktır.

Oluşturduğum kontratta 3 tane set methodu vardır. Bunlar approve, transferFrom ve transfer methodlarıdır. Diğer methodlar get methodları olup transaction kontrolü için gerekli bilgileri döndürmektedirler. 

Tokenı oluşturmak ve vitual walleta atmak için kullandığım teknolojiler:
<ul>
<li>Solidity</li>
<li>MetaMask</li>
 </ul>
 
 Solidity akıllı kontratlar yazma amacı ile ortaya çıkmış nesne tabanlı bir programlama dilidir.
 MetaMask, etherium blockchaininde işlem yapmamızı sağlayan bir sanal cüzdandır.
 
 Solidity ile yazdığımız akıllı kontratı metaMask ile kullanmak için öncelikli olarak metaMask hesabımızı solidity ile bağlamamız gerekmektedir. Bunun için solidity'de 'deploy and run' sekmesine tıklayıp environmenti injected web3 yapmanız yeterli, deploy ettiğinizde otomatik olarak metaMask hesabınız ile bağlantı kuracaktır ve işlemi onaylamanız için eklentiyi açacaktır. Onaylama işleminden sonra metaMask hesabınız solidity ile bağlanmış oluyor. Oluşturduğumuz tokenı metaMask'da tanımlamak için 'add token' butonuna tıklayıp, contrat numaranızı ilgili yere yazmanız gerekiyor. Bunun için solidity'de oluşan kontratın numarasını kopyalıyor ve yapıştırıyoruz. metaMask otomatik olarak tokenımzı tanımlıyor. Artık istediğimiz hesaba tokenı gönderebiliriz.
 
 Eğer metaMask'a tokenızı ekledikten sonra bakiyeyi 0 görüyorsanız, contratta initial tokenızı 0 yapmışsınız demektir. Eğer böyle bir sorunla karşılaşırsanız, balanceların içinde ownera (yani contrat sahibine) initial değer girmeyi unutmayın. 

# new_Project
create a new project
<?php


class Books
{
    public $price;
    public $title;

    /* các hàm thành viên */
    function __construct($par1, $par2)
    {
        $this->title = $par1;
        $this->price = $par2;
    }

    function getPrice()
    {
        echo $this->price . "$" . "\n";
    }

    function getTitle()
    {
        echo $this->title . "\n";
    }
}

class inherent
{
    public $author;
    public $publisher;

    function __construct($parr1, $parr2)
    {
        $this->author = $parr1;
        $this->publisher = $parr2;
    }
    function getAuthor()
    {
        echo $this->author . "\n";
    }

    function getPublisher()
    {
        echo $this->publisher . "\n";
    }
}
class NewBooks1 extends Books
{

}
class NewBooks2 extends inherent
{

}
$english = new NewBooks1('Practive and Grammar', 20);
$toanCaoCap = new NewBooks1("Toan Cao Cap 1", 15);
$thuPhatVoTuyen = new NewBooks1("Hệ thống thu và phát vô tuyến", 18);

$tieuThuyet =new NewBooks2("marie","Kim Dong");
$antena= new NewBooks2("Ts.Dang The Ngoc","Giao Duc");
$giaitich = new NewBooks2("Ts. Pham Ngoc Anh","Giao Duc");

$thuPhatVoTuyen->getTitle();
$thuPhatVoTuyen->getPrice();
$antena->getAuthor();
$antena->getPublisher();

$toanCaoCap->getTitle();
$toanCaoCap->getPrice();
$giaitich->getAuthor();
$giaitich->getPublisher();

$english->getTitle();
$english->getPrice();
$tieuThuyet->getAuthor();
$tieuThuyet->getPublisher();

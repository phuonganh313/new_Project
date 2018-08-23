<?php

class sapXepMang
{
    protected $_arrSort;

    function __construct(array $arrSort)
    {
        $this->_arrSort=$arrSort;
    }

    function sapXep(){
        $sorted= $this->_arrSort;
        sort($sorted);
        return $sorted;
    }
}
$arrSorted= new sapXepMang(array(1,2,3,4,56,"a"));
print_r($a
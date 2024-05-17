# oop-1-3
<?php

// auteur: onurkan yalciner

class Product
{
    // properties
    public $name = "soda";
    private $price;

    // methods
    public function showProduct()
    {

        echo "<br> Name: " . $this->name . "<br>";
        echo "<br> Price: " . $this->getPrice() . "<br>";
    }

    public function setPrice($setPrice)
    {

        $this->price = $setPrice;
    }

    public function getPrice()
    {

        return $this->price;
    }
}

$pepsi = new Product();
$pepsi->name = "Pepsi";
$pepsi->setPrice(1.19);

// var_dump($pepsi);
$pepsi->showProduct();


$fanta = new Product();
$fanta->name = "Fanta";
$fanta->setPrice(1.09);

// var_dump($fanta);
$fanta->showProduct();


$sprite = new Product();
$sprite->name = "Sprite";
$sprite->setPrice(1.29);

// var_dump($sprite);
$sprite->showProduct();


$sisi = new Product();
$sisi->setPrice(1.29);

// var_dump($sisi);
$sisi->showProduct();

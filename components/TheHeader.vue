<template>
    <header class="Header">
        <div class="Header__contacts">
            <div class="container">
                <div class="row">
                    <div class="col-md-6 text-left Header__contacts__items">
                        <a href=""><i class="text-danger fa fa-map-marker"></i>&nbsp; Алматы</a>
                        <a href="" class="phone"><i class="text-danger fa fa-phone"></i>&nbsp; +7 (727) 356-99-21</a>
                        <a href=""><i class="text-danger fa fa-phone"></i>&nbsp; +7 (812) 424-43-62</a>
                    </div>
                    <div class="col-md-6 text-right">
                        <Btn is_link="1" href="#">Важно</Btn>

                        <Btn is_link="1" href="#" label="Добавить объявление">Важно</Btn>
                    </div>
                </div>
            </div>
        </div>
        <div class="Header__menu">
            <div class="container">
                <div class="row">
                    <div class="col-md-2">
                        <img src="/logo.svg" width="100%" alt="logo" />
                    </div>
                    <div class="col-md-9">
                        <menu class="Header__menu__links">
                            <a href="">Купить</a>
                            <a href="">Продать</a>
                            <a href="">Квартиры</a>
                            <a href="">Дома/участки</a>
                            <a href="">Коммерция</a>
                            <a href="">Новостройки</a>
                            <a href="">Скоростная Ипотека</a>
                            <a href="">Онлайн Оценка</a>
                            <a href="">Работа</a>
                            <a href="">Франшиза</a>
                            <a href="">Выгоды для Продавца</a>
                            <a href="">Выгоды для Покупателя</a>
                        </menu>
                    </div>
                    <div class="col-md-1">
                        icons
                    </div>
                </div>
            </div>
        </div>
    </header>
</template>

<style scoped lang="scss">
    .Header {
        width: 100%;
    }

    .Header__contacts {
        padding: 20px 0px;
        font-size: 16px;
        color: #000;
        font-weight: bold;
        background: #F0F0F2;
    }

    .phone {
        border-right: 1px solid #c2c2c2;
        margin-right: 20px;
    }

    .Header__contacts a {
        color: #000;
        padding-right: 20px;
    }

    .Header__menu {
        padding: 25px 0px;
    }

    .Header__menu__links {
        margin: 0;
    }

    .Header__menu__links a {
        color: #7a7a87;
        display: inline-block;
        padding: 5px;
        font-size: 14px;
        text-decoration: none;
    }

    .Header__menu__links a:hover {
        color: #AA0001;
    }
</style>
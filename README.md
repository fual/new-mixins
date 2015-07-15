# new-mixins
Мои миксины для Sass

1) Миксин для создания стилей
Указываешь диапазон
{code}
font-size-styles($startSize: 10, $endSize : 30)
{code}
 Получаешь набор классов вида
{code}
.__f12 {
 font-size: 12px
}
{code}

2) Mixin для штрих-кода gradient-barcode

  .test {
    width 310px;
    height 20px;
    position: relative;
    text-align: center;
    color: $white;

    //box-shadow: -3px 0px 0px 1px #0d3f72 , -6px 0px 0px 1px transparent, -10px 0px 0px 1px #0d3f72 ;
    &:before {
      @include gradient-barcode(#0d3f72, 2 3 2 10 7 5 7 5 2 4 4 3 4 3 7 2 4 4 2);
      height: inherit;
      content: '';
      display: block;
      float: left;
    }
   }

   <div class="test"></div>

2) 



3) Миксины для маргинов и паддингов

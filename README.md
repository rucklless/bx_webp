# bx_webp

Инициализируем класс

use Bas\Pict;

Далее вызовем метод для генерации webp из детальной картинки

<img src="<?=Pict::getResizeWebpSrc($arResult['DETAIL_PICTURE'], 500, 500)?>" alt="<?=$arResult['DETAIL_PICTURE']['ALT']?>" height="<?=Pict::getLastHeight()?>" width="<?=Pict::getLastWidth()?>">

Либо используя тег <picture>

<picture>
    <source type="image/webp" srcset="<?=Pict::getResizeWebpSrc($arResult['DETAIL_PICTURE'], 500, 500)?>">
    <img src="<?=Pict::getResizeSrc($arResult['DETAIL_PICTURE'], 500, 500)?>" alt="<?=$arResult['DETAIL_PICTURE']['ALT']?>" height="<?=Pict::getLastHeight()?>" width="<?=Pict::getLastWidth()?>">
</picture>


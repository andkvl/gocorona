Фрилансер по жизни https://youtu.be/sohdv21BVNI


beginning: 04.07.2022
ending:

 около 1:24:00 - гамбургер
 около 1:31:00 - скрыть текст в картике на лого
  !!! Нужно убрать в этом изображении max-width: 100%;
 около 1:32:00 - меню (для маленьких разрешений)
 около 1:38:00 - :target
    :target смотри в _hamburger.scss


!!! В andkvl привести в порядок base and constants

Трюки с псевдоклассом :target
  http://prgssr.ru/development/tryuki-s-psevdoklassom-target.html

Адаптивное (отзывчивое) CSS свойство. Как быстро адаптировать элементы.
  https://youtu.be/eaOAY0vIB4U

Для img указывает vertical-align: top;
        text-align: center;
В base display: block; => text-align: center; не ставит по-центру => inline-block

!!! Соотношение высоты к ширине (padding-bottom = h / w * 100%);
  При применении этого способа (здесь это flex-элемент в flex-контейнере) padding будет расчитываться от width Главной оси всего родителя (flex-контейнера в данном случае (.experts__body); например, width = 1057px => pb = 1057*58% = 613px).

.experts__body {
  display: flex;
}
.experts__video {
  flex: 0 1 50%;
  position: relative;
  padding-bottom: 58%;
  > iframe {
    position: absolute;
    width: 100%;
    height: 100%;
    object-fit: cover;
    top: 0;
    left: 0;
  }
}
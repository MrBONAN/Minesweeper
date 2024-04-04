# Minesweeper
Игра на Jack
Стандартная игра Сапёр с полем 16 на 16 клеток
Самые интересные части:
> Реализован рандом, но надо задавать изначальный seed. Были идеи, как можно реализовать рандомный seed, но уже было мало времени и сил
> Реализован HashSet Вроде должен работать, но проверки не было. Изначально он нужен был для рекурсивного открытия клеток, но, оказалось, можно и без него
> Реализован List для HashSet, но HashHset не использовался, поэтому не использовался и List. В принципе, у него есть удобные команды Add и Contains, может пригодится кому-нибудь

Возможные улучшения:
> Добавить возможность начать новую игру, не перезапуская текущую
> Добавить нажатие на клетку с цифрой и, если все флажки уже поставлены вокруг текущей клетки, открыть оставшиеся закрытые поля вокруг
> Изменить момент генерации поля, чтобы seed рандома зависел от того, через сколько тиков компьютера игрок нажал на открытие первой клетки, так появится псевдорандом + можно отслеживать нажатиия WASD для дополнительного рандома. Возможно, что с данным seed поле не сгенерируется (такого ещё не было, но всё может быть) из-за того, что при расстановке мин будут происходить постоянные коллизии с уже поставленными минами. В таком случае сделать ограничение на количество попыток поставить мину, иначе просто установить новый seed рандома
> Добавить методы для очистки памяти.

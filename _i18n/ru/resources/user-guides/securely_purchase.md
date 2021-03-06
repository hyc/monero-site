{% assign version = '1.1.0' | split: '.' %}
{% include disclaimer.html translated="true" version=page.version %}
## О приобретении и безопасном хранении Monero

Это руководство по приобретению и безопасному хранению Monero по состоянию на июнь 2017 года.

#### Шаг 1. Покупка Bitcoin

Существует множество способов приобретения Bitcoin. Двумя относительно надежными компаниями в настоящее время являются Xapo <http://www.xapo.com/> и Coinbase <http://www.coinbase.com/>. Сам процесс включает в себя загрузку ваших персональных данных (данных удостоверения личности государственного образца, паспорта, и т. д.) и занимает приблизительно от 2 до 10 дней (случается, что и больше). Перед совершением крупной закупки следует проверить репутацию продавца на Reddit. Xapo использует телеграфные денежные переводы, а Coinbase — банковские переводы (ACH в USA). Xapo, пожалуй, работает быстрее, чем Coinbase. При этом Coinbase поддерживает проведение небольших «мгновенных» сделок с использованием дебетовых карт. Однако за данную опцию придётся заплатить довольно крупную комиссию. После приобретения Bitcoin его можно конвертировать в Monero.

#### Шаг 2. Загрузка и создание бумажного кошелька на безопасном изолированном компьютере

Необходимо загрузить генератор бумажных кошельков. Это можно сделать по ссылке: https://moneroaddress.org. После этого генератор следует скопировать на USB-накопитель (прямая ссылка: https://github.com/moneromooo-monero/monero-wallet-generator/archive/master.zip).

Затем необходимо разархивировать и открыть генератор (monero-wallet-generator.html) в веб-браузере на изолированном компьютере, который либо до этого не использовался, либо на который установлена только ОС.

Бумажный кошелек должен иметь четыре важных элемента.

Публичный адрес Monero
убличный адрес используется для получения средств на кошелек. Его можно передать любому лицу, собирающемуся отправить вам средства.

Мнемоническая фраза Monero
Мнемоническая фраза представляет собой легко читаемый человеком способ обеспечения безопасности целого кошелька. Её будет достаточно для восстановления кошелька в будущем.

Приватный ключ траты Monero
Приватный ключ траты используется для перевода средств с кошелька.

Приватный ключ просмотра Monero
Приватный ключ просмотра необходим для наблюдения за входящими на кошелек транзакциями. Обычно он используется для настройки кошелька формата «view-only», который позволяет только просматривать входящие в блокчейн транзакции в режиме реального времени по мере того, как они отправляются на холодный кошелёк.

На данном этапе у пользователя имеется множество опций. Можно создать бумажный кошелек, сохранить его в формате PDF или в текстовом формате на USB-носителе, CD/DVD диске и т. д. Скорее всего, потребуется не менее двух-трёх копий, которые будет можно хранить в безопасности в разных местах. При хранении на цифровых носителях требуется защитить их надёжным паролем. При хранении на бумаге не следует показывать кошелёк лицам, способным либо запомнить ваш ключ, состоящий из 25 слов, либо сфотографировать его без вашего разрешения. Отправка фотографии кошелька третьим лицам может означать потерю всех ваших средств.

Какой бы способ вы не выбрали, следует убедиться в том, что на устройстве, которое было использовано, не осталось ни одной копии кошелька Monero. Вам может потребоваться полное удаление кошелька, если вы сохранили его на диске, а также убедиться в том, что ваш принтер не сохранил каких-либо копий в памяти.

*При потере доступа к вашему бумажному кошельку Monero ни вы, ни кто-либо другой не сможет когда-нибудь снова получить его. Восстановить кошелёк вы уже никогда не сможете!

#### Сноска на полях
Опция шифрования мнемонической фразы XMR:
https://xmr.llcoins.net/
Загрузите html-страницу и разместите ее на изолированном компьютере. Далее выберите Encrypt/Decrypt Mnemonic Seed [Зашифровать/расшифровать мнемоническую фразу] и убедитесь, что используете CN Add с надёжным паролем. Спасибо пользователю manicminer5.



#### Шаг 3. Перевод Bitcoin в Monero и отправка на бумажный кошелек Monero

Сядьте за компьютер с подключением к интернету и перейдите по адресу www.shapeshift.io. Выберите раздел Deposit Bitcoin [Внести Bitcoin] и Receive Monero [Получить Monero] (и побыстрее).

Нажмите Continue [Продолжить].

Your Monero Address [Адрес Monero] (публичный адрес Monero вашего бумажного кошелька)
Введите публичный адрес Monero вашего бумажного кошелька в поле Your Monero Address (Ваш адрес Monero). Хотя, стоп! Ведь если ваш публичный адрес находится на изолированном компьютере (верно же?), вы не сможете скопировать и вставить что бы то ни было… Тогда либо перепишите его от руки, либо придется взять чистый USB-накопитель и скопировать на него публичный адрес.

Refund Address [Адрес возмещения] (публичный адрес Bitcoin, на который вы можете получать средства)
Введите ваш адрес Bitcoin, на который будут возвращены средства при возникновении каких-либо проблем с транзакцией. Очень важно указать публичный адрес Bitcoin, который вы либо полностью контролируете, либо на который вы сможете получить средства. В случае с Xapo и Coinbase он будет называться Receive Address [Адрес получения] и может периодически меняться.

Payment ID [Идентификатор платежа]
При отправке средств на принадлежащий вам кошелек Monero или бумажный кошелек Monero данное поле следует оставить незаполненным.

Согласитесь с условиями и переместите слайдер до поля "Reusable Address" (Многоразовый адрес).  

Нажмите "Start Transaction" [Начать транзакцию].

Deposit Address [Адрес депозита] (публичный адрес Bitcoin обменника Shapeshift.io, предназначенный исключительно для получения средств)
Скопируйте адрес депозита из появившегося всплывающего окна в буфер обмена (используя клавиши Ctrl+C или через меню: Правка–Копировать). По этому адресу произойдёт отправка Bitcoin из Xapo / Coinbase в Shapeshift.io.

Теперь необходимо вернуться в свою учётную запись Xapo или Circle и найти кнопку Transfer [Перевести] или Send [Отправить]. Следует вставить адрес депозита Bitcoin в поле Destination [Адресат] и ввести сумму Bitcoin, которую требуется перевести в Monero. Сумма должна находиться в пределах минимального и максимального депозита, определяемого Shapeshift.io. После этого можно нажать Send (Отправить) и, в случае необходимости, подтвердить транзакцию.

После начала передачи через Xapo / Coinbase произойдёт задержка, связанная с вводом транзакции в блокчейн Bitcoin и ожиданием подтверждения. Это может занять от нескольких минут до нескольких часов. Факт отправки платежа можно проверить через адрес депозита Shapeshift.io на blockchain.info. Здесь должна отобразиться ваша транзакция Shapeshift.io.

После подтверждения транзакции Shapeshift.io начнёт обмен Bitcoin (BTC) на Monero (XMR) через одну из бирж, и по завершении обмена отправит Monero на адрес вашего холодного бумажного кошелька! Это также может занять от нескольких минут до нескольких часов. В случае возникновения проблем следует обратиться в Shapeshift.io. У них хорошая служба поддержки.

Когда на веб-странице Shapehift.io появится информация, подтверждающая завершение транзакции, Monero уже будут в вашем бумажном кошельке!


#### Примечания и способы верификации средств
Ввиду того, что блокчейн Monero анонимен и не допускает отслеживания транзакций, вы не сможете при просмотре вашего публичного адреса Monero удостовериться в получении средств, как можно было бы сделать в случае с Bitcoin. Это хорошо с точки зрения анонимности, но плохо с точки зрения создаваемых неудобств.

Чтобы безопасно проверить получение средств на кошелёк, необходимо установить кошелек, предназначенный исключительно для просмотра (view-only). Здесь пригодится ключ просмотра. Для создания такого кошелька ознакомьтесь с: [Кошелек только для просмотра]({{site.baseurl}}/resources/user-guides/view_only.html)

Для подтверждения того, что средства *по-прежнему находятся* вашем кошельке и не были потрачены, требуется создать холодный кошелек при помощи вашего мнемонического ключа (для всех ваших средств) на изолированном компьютере с актуальной копией блокчейна Monero. После завершения в целях безопасности придётся либо стереть кошелек, либо подключить его к Интернету, после чего он станет горячим кошельком.

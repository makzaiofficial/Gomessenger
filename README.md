# Gomessenger
Описание: Это официальный репозиторий для GOmessenger — мессенджера для Android. Здесь представлен исходный код приложения, позволяющий разработчикам изучать, вносить изменения или создавать собственные версии приложения.

Лицензия: Проект является открытым и распространяется под лицензией GNU General Public License v2.0.

Основные функции:
Быстрая и безопасная передача сообщений.

Поддержка групповых чатов, каналов и секретных чатов.

Шифрование данных для защиты конфиденциальности.

Возможность создания собственных сборок приложения.

# Для разработчиков:
Репозиторий предоставляет возможность изучить код GOmessenger, внести свой вклад в разработку или создать кастомную версию приложения.
# Руководство по компиляции
Примечание: Для поддержки воспроизводимых сборок это репозиторий содержит фиктивный release.keystore, google-сервисы.json и заполненные переменные внутри BuildVars.java. Перед публикацией ваших собственных APK-файлов, пожалуйста, замените все эти файлы на свои собственные.

Вам потребуются Android Studio 3.4, Android NDK rev. 20 и Android SDK 8.1

Загрузите исходный код Gomessenger с сайта https://github.com/makzaiofficial/Gomessenger
Скопируйте свой release.keystore в TMessagesProj/config
Заполните RELEASE_KEY_PASSWORD, RELEASE_KEY_ALIAS, RELEASE_STORE_PASSWORD в gradle.properties, чтобы получить доступ к вашему release.keystore
Перейдите по ссылке https://console.firebase.google.com /, создайте два приложения для Android с идентификаторами приложений org.telegram.messenger и org.telegram.messenger.beta, включите firebase messaging и загрузите google-services.json, который следует скопировать в ту же папку, что и TMessagesProj.
Откройте проект в Studio (обратите внимание, что он должен быть открыт, а не импортирован).
Введите значения в поле TMessagesProj/src/main/java/org/telegram/messenger/BuildVars.java – для каждой из переменных есть ссылка, показывающая, где и какие данные можно получить.
Вы готовы к компиляции Gomessenger.

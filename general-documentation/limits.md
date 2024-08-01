### Загальні Помилки Веб-Служби

**Для перегляду актуальної документації перейдіть у розділ ["Документація"](https://developers.ria.com/docs/)**

Певні поширені помилки будуть повернуті стандартним способом з усіх веб-сервісів API RIA.com. Крім того, деякі повідомлення про помилки можуть бути специфічними для деяких сервісів (дивитись документацію для конкретного сервісу). Нижче описано поширені помилки:

<table>
<thead>
                <tr>
                    <th class="doc-parameters-name" scope="col" style="width: 100px;">Error Code</th>
                    <th class="doc-parameters-name" scope="col" style="width: 100px;">HTTP Status Code</th>
                    <th class="doc-parameters-required" scope="col">Опис</th>
                </tr>
                </thead>
                <tbody>
                <tr>
                    <th class="doc-parameter-name" scope="row">API_KEY_MISSING</th>
                    <td class="doc-parameter-name">403</td>
                    <td class="doc-parameter-description">
                        API ключ не було вказано. Детальніше про
                        <a href="https://api-docs-v2.readthedocs.io/ru/latest/general-documentation/api_key.html">використання</a> API ключа дивитись у розділі "Використання API Key" .
                    </td>
                </tr>
                <tr>
                    <th class="doc-parameter-name" scope="row">API_KEY_INVALID</th>
                    <td class="doc-parameter-name">403</td>
                    <td class="doc-parameter-description">
                        Було вказано неправильний ключ API. Переконайтеся, що було вказано коректний API ключ, або
                        <a href="https://developers.ria.com/signup">зареєструйтеся</a> для отримання ключа.
                    </td>
                </tr>
                <tr>
                    <th class="doc-parameter-name" scope="row">API_KEY_DISABLED</th>
                    <td class="doc-parameter-name">403</td>
                    <td class="doc-parameter-description">
                        API ключ було вимкнено адміністратором. Будь ласка
                        <a href="https://developers.ria.com/contact">зв'яжіться з нами</a> для допомоги.
                    </td>
                </tr>
                <tr>
                    <th class="doc-parameter-name" scope="row">API_KEY_UNAUTHORIZED</th>
                    <td class="doc-parameter-name">403</td>
                    <td class="doc-parameter-description">
                       API ключ не авторизований для доступу до цього сервісу. Будь ласка
                        <a href="https://developers.ria.com/contact">зв'яжіться з нами</a> для допомоги.
                    </td>
                </tr>
                <tr>
                    <th class="doc-parameter-name" scope="row">API_KEY_UNVERIFIED</th>
                    <td class="doc-parameter-name">403</td>
                    <td class="doc-parameter-description">
                        API ключ не підтверджено. Перевірте свою електронну пошту для підтвердження API ключа. Будь ласка
                        <a href="https://developers.ria.com/contact">зв'яжіться з нами</a> для допомоги.
                    </td>
                </tr>
                <tr>
                    <th class="doc-parameter-name" scope="row">HTTPS_REQUIRED</th>
                    <td class="doc-parameter-name">400</td>
                    <td class="doc-parameter-description">Запити до цього API мають бути зроблені за HTTPS протоколом.                                                            Переконайтеся, будь ласка, що Ви використовуєте HTTPS протокол для Вашого                                                           запиту.
                    </td>
                </tr>
                <tr>
                    <th class="doc-parameter-name" scope="row">OVER_RATE_LIMIT</th>
                    <td class="doc-parameter-name">429</td>
                    <td class="doc-parameter-description">
                        Перевищено ліміт запитів для цього API ключа.
                        <a href="https://developers.ria.com/contact">Зв'яжіться з нами</a> для отримання додаткової інформації про
                        <a href="https://api-docs-v2.readthedocs.io/ru/latest/general-documentation/rate_limits.html"> ліміти веб-сервісів</a> .
                    </td>
                </tr>
                <tr>
                    <th class="doc-parameter-name" scope="row">NOT_FOUND</th>
                    <td class="doc-parameter-name">404</td>
                    <td class="doc-parameter-description">
                       Не вдалося знайти API за цією URL-адресою. Перевірте свій URL.
                    </td>
                </tr>
                </tbody>
            </table>

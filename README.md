# lecture_async
## Synchronous
> Synchronous Javascript: As the name suggests, synchronous execution is when statements are executed one at a time in the order in which they appear. Each statement waits for the previous to finish, also known as “blocking”
>
> Синхронный Javascript: как следует из названия, синхронное выполнение — это когда операторы выполняются по одному в том порядке, в котором они появляются. Каждый оператор ожидает завершения предыдущего, что также называется «блокировкой».

![](/images/sync.webp)

## Asynchronous
> Asynchronous Javascript: In an asynchronous, or non-blocking, environment, code can be executed immediately instead of waiting for the previous to finish. Having code that runs asynchronously allows a user to fetch data from the server, execute a function with a delay, and deal with multiple requests simultaneously. This helps to reduce the waiting time for the user.
>
> Асинхронный Javascript: в асинхронной или неблокирующей среде код может выполняться немедленно, а не ждать завершения предыдущего. Наличие кода, работающего асинхронно, позволяет пользователю получать данные с сервера, выполнять функцию с задержкой и обрабатывать несколько запросов одновременно. Это помогает сократить время ожидания пользователя.

> The most common triggers for asynchronous Javascript operations are:
>
> 1) Callback
>
> 2) Promises
>
> 3) Async/Await 
>

> Callbacks are functions that are passed as arguments to other functions and are executed when the called function completes its task. Callbacks can be used to handle asynchronous operations by passing a callback function to an asynchronous method, which then calls the callback function when the operation is complete.
>
> Обратные вызовы — это функции, которые передаются в качестве аргументов другим функциям и выполняются, когда вызываемая функция завершает свою задачу. Обратные вызовы можно использовать для обработки асинхронных операций путем передачи функции обратного вызова асинхронному методу, который затем вызывает функцию обратного вызова после завершения операции.

![](/images/callback.jpg)


> In JavaScript, a promise is a good way to handle asynchronous operations. It is used to find out if the asynchronous operation is successfully completed or not.
>
> В JavaScript обещание — это хороший способ обработки асинхронных операций. Он используется, чтобы узнать, успешно ли завершена асинхронная операция или нет.

> A promise may have one of three states:
>
> 1) Pending - В ожидании
> 2) Resolve - Выполнено
> 3) Rejected - Рад карда шуд

## Promise 

> Promise – это специальный объект, который содержит своё состояние. Вначале pending («ожидание»), затем – одно из: Resolve («выполнено успешно») или rejected («выполнено с ошибкой»).
>
> На promise можно навешивать колбэки двух типов:
> 1) onResolve – срабатывают, когда promise в состоянии «выполнен успешно».
> 2) onRejected – срабатывают, когда promise в состоянии «выполнен с ошибкой».

> Конструктор Promise() принимает функцию в качестве аргумента. Функция также принимает две функции resolve() и reject().

> Если обещание успешно возвращается, вызывается функция resolve(). И, если возникает ошибка, вызывается функция reject().

![](/images/promise.jpg)

### Try...Catch

> Конструкция try...catch пытается выполнить инструкции в блоке try, и, в случае ошибки, выполняет блок catch.
>
> Конструкция try содержит блок try, в котором находится одна или несколько инструкций (Блок ({} ) обязательно должен присутствовать, даже если выполняется всего одна инструкция), и хотя бы один блок catch или finally. Таким образом, есть три основные формы конструкции try:

![](/images/try.jpg)


### Async function

> Объявление async function определяет асинхронную функцию, которая возвращает объект AsyncFunction.
>
> После вызова функция async возвращает Promise. Когда результат был получен, Promise завершается, возвращая полученное значение. Когда функция async выбрасывает исключение, Promise ответит отказом с выброшенным (throws) значением.

### Axios

> GET

> Axios - это HTTP-клиент, основанный на Promise для node.js и браузера. Он может работать в браузере и node.js с той же базой кодов.
![](/images/Screenshot_15.png)

> Delete 
![](/images/Screenshot_1.png)
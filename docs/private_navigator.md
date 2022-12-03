<style>
    .protected {
        border: 5px solid black;
        border-radius: 5px;
    }
    .protected__content {
        padding: 24px 28px;
    }
    .protected__content__heading {
        font-size: 16px;
        font-weight: 500;
        margin: 0 0 12px;
        line-height: 1;
    }
    .protected__alert {
        display: none;
        border-bottom: 1px solid transparent;
        border-radius: 3px 3px 0 0;
        padding: 12px 14px;
        color: #a94442;
        background-color: #f2dede;
        border-color: #ebccd1;
    }
    .protected__content__input {
        display: block;
        border: solid 1px #ccc;
        padding: 12px 14px;
        -webkit-box-shadow: 0 2px 3px 0 rgba(0,0,0,0.1);
        box-shadow: 0 2px 3px 0 rgba(0,0,0,0.1);
        font-size: 16px;
        width: 100%;
        border-radius: 3px;

        margin-bottom: 12px;
    }
    .protected__content__input:focus {
        outline: none;
        border-color: #228843;
    }
    .protected__content__btn {
        background-color: #228843;
        border-radius: 3px;
        cursor: pointer;
        border: none;
        color: #fff;
        padding: 12px 14px;
        font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Roboto", "Oxygen", "Ubuntu", "Cantarell", "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif;
        font-weight: 500;
        font-size: 16px;

    }
    .protected__content__btn:hover {
        background-color: #1C6D36;
    }
</style>

<div class="protected">
    <div class="protected__alert" id="alert">Das eingegebene Passwort ist falsch!</div>
    <div class="protected__content">
        <h1 class="protected__content__heading" style="font-size:24px;">Für den Zugriff auf private Inhalte ist ein Passwort erforderlich.</h1>
        <input class="protected__content__input" id="password-input" type="password" placeholder="Passwort"/>
        <button onclick="login_private(document.querySelector('#password-input').value)" id="password-button" type="button" class="protected__content__btn">Weiter</button>
    </div>
</div>


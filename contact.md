---
layout: default
title: Contacto
permalink: /contacto/
---

<h1>{{ page.title }}</h1>

<form action="https://formspree.io/f/mqapnkbo" method="POST">
  <label for="nombre" class="form-label">Nombre:</label>
  <input type="text" id="nombre" name="nombre" required maxlength="50" class="form-input">

  <label for="mensaje" class="form-label">Mensaje:</label>
  <textarea id="mensaje" name="mensaje" required maxlength="500" class="form-input"></textarea>

  <button type="submit" class="btn-enviar">Enviar</button>
</form>

<style>
  form {
    max-width: 500px;
    margin: 0 auto;
  }
  label, input, textarea, button {
    display: block;
    width: 100%;
    margin-bottom: 1rem;
  }
  textarea {
    height: 150px;
  }
</style>
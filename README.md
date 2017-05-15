# formulario-Django
Começando edição de formulário em Django

{% extends "base.html" %}
{% load static %}
{% block content %}

   <div id="telaCadastro">
      <h1 class="cabecalhoCadastro">Cadastro de Usuário</h1>
      <p class="cabecalhoCadastro"><i>Informe seus dados para prosseguir</i></p>
      <div class="formulario">
        <label>Nome completo<em>*</em></label><br>
        <input class="inputCadastro" type="text" placeholder="Digite o nome"><br><br>

        <label>CPF <em>*</em></label><br>
        <input class="inputCadastro" type="text" placeholder="Digite o CPF"><br><br>

        <label>Email </label><br>
        <input class="inputCadastro" type="text" placeholder="Digite o Email"><br><br>

        <label>Estado<em>*</em></label><br>
        <select>
          <option value="opcao1">Opção 1</option>
          <option value="opcao2">Opção 2</option>
          <option value="opcao3">Opção 3</option>
          <option value="opcao4">Opção 4</option>
          <option value="opcao5">Opção 5</option>
          <option value="opcao6">Opção 6</option>
          <option value="opcao7">Opção 7</option>
          <option value="opcao8">Opção 8</option>
        </select><br><br>

        <label>Cidade <em>*</em></label><br>
        <select>
          <option value="opcao1">Opção 1</option>
          <option value="opcao2">Opção 2</option>
          <option value="opcao3">Opção 3</option>
          <option value="opcao4">Opção 4</option>
          <option value="opcao5">Opção 5</option>
          <option value="opcao6">Opção 6</option>
          <option value="opcao7">Opção 7</option>
          <option value="opcao8">Opção 8</option>
        </select><br><br>

        <label>Universidade</label><br>
        <input class="inputCadastro" type="text" placeholder="Informe a universidade"><br><br>

        <a class="linkGeral linkCancelar" href="{% url'core:home'%}">Cancelar cadastro</a><br>
        <a href="usuariosenha.html"><button class="buttonprosseguir" type="submit" >Prosseguir</button></a>
      </div>
    </div>
    {% endblock %}

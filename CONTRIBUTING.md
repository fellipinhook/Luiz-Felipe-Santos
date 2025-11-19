# Guia de Contribuição

Obrigado por se interessar em contribuir para o **Sistema Omnichannel para Clínica Médica**! Este documento fornece diretrizes e instruções para contribuir com o projeto.

## 📋 Código de Conduta

Todos os contribuidores devem seguir nosso Código de Conduta:
- Seja respeitoso com outros contribuidores
- Aceite críticas construtivas
- Foque no que é melhor para a comunidade
- Mostre empatia com outros membros da comunidade

## 🚀 Como Contribuir

### 1. Reportar Bugs

Se encontrar um bug, abra uma issue com:
- **Título descritivo**: Descreva o problema brevemente
- **Descrição detalhada**: Explique o comportamento esperado vs. atual
- **Passos para reproduzir**: Como reproduzir o problema
- **Screenshots**: Se aplicável
- **Ambiente**: Navegador, SO, versão

### 2. Sugerir Melhorias

Para sugerir uma melhoria:
- Use um **título descritivo**
- Forneça uma **descrição detalhada** da melhoria
- Liste alguns **exemplos** de como a melhoria funcionaria
- Explique por que essa melhoria seria útil

### 3. Submeter Pull Requests

#### Pré-requisitos
- Tenha Git instalado
- Tenha uma conta GitHub
- Fork o repositório

#### Processo

1. **Fork o repositório**
   ```bash
   git clone https://github.com/seu-usuario/omnichannel-clinica.git
   cd omnichannel-clinica
   ```

2. **Crie uma branch para sua feature**
   ```bash
   git checkout -b feature/sua-feature
   # ou para bugfix
   git checkout -b bugfix/seu-bugfix
   ```

3. **Faça suas mudanças**
   - Mantenha o código limpo e bem documentado
   - Siga as convenções de código existentes
   - Teste suas mudanças

4. **Commit suas mudanças**
   ```bash
   git add .
   git commit -m "Descrição clara das mudanças"
   ```

5. **Push para sua branch**
   ```bash
   git push origin feature/sua-feature
   ```

6. **Abra um Pull Request**
   - Descreva as mudanças claramente
   - Referencie qualquer issue relacionada
   - Aguarde revisão

## 📝 Convenções de Código

### HTML
- Use indentação de 4 espaços
- Use nomes de classe descritivos
- Mantenha a estrutura semântica

### CSS
- Use variáveis CSS para cores e espaçamento
- Organize por seções com comentários
- Use nomes de classe BEM quando apropriado
- Mobile-first approach

### JavaScript
- Use camelCase para variáveis e funções
- Adicione comentários para lógica complexa
- Use const/let ao invés de var
- Evite console.log em produção

## 🔍 Padrões de Commit

Use mensagens de commit descritivas:

```
[TIPO] Descrição breve

Descrição mais detalhada se necessário.

Fixes #123
```

Tipos de commit:
- **feat**: Nova funcionalidade
- **fix**: Correção de bug
- **docs**: Mudanças na documentação
- **style**: Mudanças de formatação
- **refactor**: Refatoração de código
- **test**: Adição ou mudança de testes
- **chore**: Mudanças em build, dependências, etc.

## 📚 Documentação

Ao adicionar novas funcionalidades:
- Atualize o README.md
- Atualize o GUIA_USO.md se necessário
- Adicione comentários no código
- Atualize a ARQUITETURA.md se mudou a estrutura

## 🧪 Testes

Antes de submeter um PR:
- Teste em diferentes navegadores
- Teste em dispositivos móveis
- Verifique responsividade
- Teste a funcionalidade completa

## 📞 Comunicação

- **Issues**: Para bugs e sugestões
- **Discussions**: Para perguntas e ideias
- **Pull Requests**: Para contribuições de código

## ✅ Checklist para PR

- [ ] Código segue as convenções do projeto
- [ ] Documentação foi atualizada
- [ ] Testei em múltiplos navegadores
- [ ] Testei em dispositivos móveis
- [ ] Não há console.log ou código de debug
- [ ] Commit messages são descritivas

## 🎓 Recursos Úteis

- [Git Documentation](https://git-scm.com/doc)
- [GitHub Flow](https://guides.github.com/introduction/flow/)
- [Markdown Guide](https://www.markdownguide.org/)
- [MDN Web Docs](https://developer.mozilla.org/)

## 📄 Licença

Ao contribuir, você concorda que suas contribuições serão licenciadas sob a mesma licença do projeto (MIT).

---

**Obrigado por contribuir!** 🎉

Se tiver dúvidas, abra uma issue ou entre em contato com os mantenedores.

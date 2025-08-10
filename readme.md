# 🗣️ Avatar 3D Falante (Talking 3D Avatar)

Um avatar 3D interativo que fala texto digitado pelo usuário, criado com Three.js e Web Speech API.

## ✨ Funcionalidades

- **Avatar 3D personalizado** criado com geometrias Three.js
- **Síntese de voz suave** em português brasileiro
- **Animações realistas** durante a fala (boca, cabeça, piscadas)
- **Interface intuitiva** com campo de texto e controles
- **Interação com mouse** - avatar segue o cursor sutilmente
- **Design responsivo** com visual moderno
- **Controles por teclado** (Ctrl+Enter para falar)

## 🚀 Demo

![Avatar 3D Falante](https://img.shields.io/badge/Status-Funcionando-brightgreen)

### Características do Avatar:

- Modelo humanóide com cabeça, corpo, braços e pernas
- Animações de fala sincronizadas com áudio
- Movimentos naturais e piscadas automáticas
- Iluminação dinâmica com sombras

## 🛠️ Tecnologias Utilizadas

- **Three.js r128** - Renderização 3D
- **Web Speech API** - Síntese de voz
- **HTML5/CSS3** - Interface e estilização
- **JavaScript ES6** - Lógica e animações

## 📋 Pré-requisitos

- Navegador moderno com suporte a WebGL
- Suporte à Web Speech API (recomendado: Chrome)
- JavaScript habilitado

## 🎯 Como Usar

1. **Clone ou baixe** o arquivo HTML
2. **Abra** no navegador (recomendado: Chrome para melhor qualidade de voz)
3. **Digite** sua mensagem no campo de texto
4. **Clique** em "🎤 Falar" ou pressione **Ctrl+Enter**
5. **Assista** o avatar falar sua mensagem!

## ⚙️ Configurações de Voz

O sistema automaticamente seleciona a melhor voz disponível:

- **Idioma**: Português Brasileiro (pt-BR)
- **Taxa**: 0.7 (velocidade natural)
- **Tom**: 1.1 (levemente agudo)
- **Volume**: 0.8 (suave)

### Vozes Priorizadas:

1. Google Portuguese (pt-BR)
2. Microsoft Portuguese
3. Qualquer voz em português disponível

## 🎨 Personalização

### Modificar Aparência do Avatar:

```javascript
// Cores do avatar
const bodyMaterial = new THREE.MeshLambertMaterial({ color: 0x4a90e2 }); // Corpo
const headMaterial = new THREE.MeshLambertMaterial({ color: 0xffdbac }); // Cabeça
const mouthMaterial = new THREE.MeshLambertMaterial({ color: 0x8b0000 }); // Boca
```

### Ajustar Parâmetros de Voz:

```javascript
utterance.rate = 0.7; // Velocidade (0.1 - 2.0)
utterance.pitch = 1.1; // Tom (0.0 - 2.0)
utterance.volume = 0.8; // Volume (0.0 - 1.0)
```

## 🔧 Estrutura do Projeto

```
talking-3d-avatar/
├── index.html              # Arquivo principal
├── README.md              # Documentação
└── assets/               # (futuro: modelos GLB/GLTF)
```

## 🌟 Melhorias Futuras

- [ ] Suporte a modelos GLB/GLTF externos
- [ ] Mais opções de personalização visual
- [ ] Expressões faciais adicionais
- [ ] Gestos com braços durante a fala
- [ ] Controles de velocidade/tom na interface
- [ ] Suporte a múltiplos idiomas
- [ ] Modo escuro/claro
- [ ] Export/import de configurações

## 🤝 Contribuições

Contribuições são bem-vindas! Sinta-se livre para:

1. **Fork** o projeto
2. Criar uma **feature branch** (`git checkout -b feature/nova-funcionalidade`)
3. **Commit** suas mudanças (`git commit -m 'Adiciona nova funcionalidade'`)
4. **Push** para a branch (`git push origin feature/nova-funcionalidade`)
5. Abrir um **Pull Request**

## 📝 Ideias de Branch Names

Para este projeto, sugerimos estes nomes de branch:

- `main` - Branch principal
- `feature/voice-improvements` - Melhorias na síntese de voz
- `feature/gltf-support` - Suporte a modelos GLB/GLTF
- `feature/ui-enhancements` - Melhorias na interface
- `feature/animations` - Novas animações
- `bugfix/speech-api` - Correções na API de fala
- `enhancement/mobile-support` - Suporte mobile

## 🐛 Problemas Conhecidos

- Web Speech API pode não funcionar em todos os navegadores
- Qualidade de voz varia conforme navegador e sistema operacional
- Em alguns navegadores, a primeira fala pode ter delay

## 📱 Compatibilidade

| Navegador | Web Speech API | Three.js | Status   |
| --------- | -------------- | -------- | -------- |
| Chrome    | ✅ Completo    | ✅       | 🟢 Ótimo |
| Firefox   | ⚠️ Limitado    | ✅       | 🟡 Bom   |
| Safari    | ⚠️ Limitado    | ✅       | 🟡 Bom   |
| Edge      | ✅ Completo    | ✅       | 🟢 Ótimo |

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

## 👨‍💻 Autor

Criado com ❤️ para demonstrar as possibilidades do Three.js com Web Speech API.

# 📚 Assistant de Révision IA (RAG Local)

> Une solution d'IA souveraine pour interroger ses cours de CY Tech en toute confidentialité.

## 🌟 Points Forts
- 🔒 **100% Local :** Aucune donnée ne quitte votre machine (RGPD compliant).
- 🧠 **Conscience du Contexte :** Répond précisément grâce à vos documents PDF.
- ⚡ **Performance :** Optimisé pour tourner sur un PC portable standard.

## 🛠️ Architecture
```mermaid
graph LR
  A[PDF Cours] --> B(Chunking)
  B --> C{Vector Store}
  D[Question] --> E(Retriever)
  E --> C
  C --> F(Llama 3)
  F --> G[Réponse Contextuelle]

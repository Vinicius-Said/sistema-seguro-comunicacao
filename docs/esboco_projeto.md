# Esboço do Projeto

## Objetivo
Segurança na comunicação entre funcionários.

## Tecnologias Utilizadas
- ✅ bcrypt → Hashing seguro de senhas.
- ✅ PyJWT → Autenticação via Tokens JWT.
- ✅ cryptography → Implementação de AES e RSA.

## Fluxo Básico do Sistema
1. ✅ Usuário faz cadastro (senha armazenada com bcrypt).
2. ✅ Usuário faz login (autenticado via JWT).
3. ✅ Usuário envia uma mensagem criptografada com AES.
4. ✅ Apenas o destinatário correto pode descriptografar com sua chave RSA.

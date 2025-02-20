# Proposta de Implementação

## Visão Geral
Este documento detalha a implementação das tecnologias utilizadas no sistema.

## Tecnologias e Uso
- **bcrypt** → Hash seguro de senhas para garantir a proteção dos dados de autenticação.
- **PyJWT** → Autenticação baseada em Tokens JWT para validar usuários de forma segura.
- **cryptography** → Implementação de criptografia AES para proteger mensagens e RSA para proteger chaves de criptografia.

## Etapas de Implementação

1. ✅ **Cadastro de Usuário**  
   - O usuário se cadastra fornecendo nome, e-mail e senha.  
   - A senha é armazenada como um hash seguro usando `bcrypt`.

2. ✅ **Login**  
   - O usuário faz login com e-mail e senha.  
   - O sistema verifica a senha e gera um Token JWT assinado.

3. ✅ **Criptografia de Mensagens**  
   - As mensagens enviadas são criptografadas usando **AES (modo CBC)** para garantir confidencialidade.

4. ✅ **Proteção da Chave AES**  
   - A chave AES usada para criptografia de mensagens é criptografada com **RSA** antes de ser armazenada.  
   - Apenas o destinatário correto pode descriptografar e acessar a mensagem.

## Armazenamento Seguro de Dados
- As senhas nunca são armazenadas em texto puro.
- Os tokens JWT possuem tempo de expiração e são assinados para evitar falsificação.
- As chaves privadas de RSA são mantidas seguras no servidor para evitar acessos não autorizados.

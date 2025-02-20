# Sistema-seguro-comunicacao

## Objetivo
Este projeto tem como foco **garantir a segurança na comunicação entre funcionários** através de autenticação segura e criptografia de mensagens.

## Funcionamento

1. **Cadastro de usuário**  
   - O usuário cria uma conta e sua senha é armazenada de forma segura usando `bcrypt`.

2. **Login**  
   - O usuário realiza login e recebe um **Token JWT** para autenticação no sistema.

3. **Envio de mensagens**  
   - As mensagens são criptografadas com **AES (CBC)** antes de serem enviadas.

4. **Proteção da chave AES**  
   - Para maior segurança, a chave AES utilizada na criptografia da mensagem é protegida com **RSA**, garantindo que somente o destinatário correto possa descriptografá-la.

## Segurança Implementada
- **Senhas protegidas** com hashing seguro (`bcrypt`).
- **Autenticação robusta** baseada em **Tokens JWT**.
- **Criptografia de ponta a ponta** usando **AES e RSA**.
- **Proteção contra acesso não autorizado**, garantindo que apenas usuários autorizados possam ler as mensagens.

Com essa abordagem, o sistema garante que as informações trocadas entre os usuários permaneçam protegidas contra acessos indevidos. 🚀

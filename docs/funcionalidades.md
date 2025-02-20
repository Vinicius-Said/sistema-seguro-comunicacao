# Proposta de Implementação

## Tecnologias Utilizadas
- **bcrypt** → Protege senhas.
- **PyJWT** → Autenticação com Tokens JWT.
- **cryptography** → Criptografia AES e RSA.

## Etapas de Implementação

### Cadastro de Usuário
- Senha protegida com **bcrypt**.

### Login
- Validação da senha e geração de **Token JWT**.

### Criptografia de Mensagens
- Mensagem protegida com **AES (CBC)**.

### Proteção da Chave AES
- Chave AES criptografada com **RSA**.

## Armazenamento Seguro
- **Senhas:** Apenas hashes são armazenados.
- **Mensagens:** Criptografadas antes do armazenamento.
- **Chaves AES:** Protegidas com RSA.

## Conclusão
O sistema garante segurança na comunicação usando criptografia e autenticação robustas.


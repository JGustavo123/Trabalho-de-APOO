# Modelo Conceitual – EventAcad

## Diagrama de Classes de Análise
![Diagrama de Classes](diagrama-classes.png)

## Descrição das Classes

### Usuario
- **Atributos:** idUsuario, nome, email, senha, tipo (organizador/participante)
- **Responsabilidades:** Autenticar no sistema, gerenciar perfil

### Evento
- **Atributos:** idEvento, nome, tema, local, data, horario, vagas, palestrantes
- **Responsabilidades:** Manter informações do evento

### Inscricao
- **Atributos:** idInscricao, dataInscricao, status
- **Responsabilidades:** Registrar participação do usuário em um evento

### Presenca
- **Atributos:** idPresenca, data, tipoRegistro (manual/QR)
- **Responsabilidades:** Controlar presença dos participantes

### Certificado
- **Atributos:** idCertificado, dataEmissao, arquivoPDF
- **Responsabilidades:** Emitir e disponibilizar certificado

### Relatorio
- **Atributos:** idRelatorio, tipo, dataGeracao
- **Responsabilidades:** Gerar informações sobre participação

---

**Observação:** As cardinalidades seguem o diagrama ER do estudo de caso original, adaptado para análise orientada a objetos.

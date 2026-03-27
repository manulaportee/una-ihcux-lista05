## 🧠 Heurísticas de Nielsen Aplicadas

Este projeto aplica conceitos de **IHC (Interação Humano-Computador)** e **UX em aplicações de console**, utilizando três heurísticas de usabilidade de Jakob Nielsen: **Visibilidade do Status do Sistema**, **Prevenção de Erros** e **Estética e Design Minimalista**.

---

### ✅ 1. Visibilidade do Status do Sistema

A heurística de visibilidade do status garante que o usuário saiba o que está acontecendo durante o uso do sistema.

No código, isso é aplicado quando o programa informa etapas do processamento:

```csharp
Console.WriteLine("\n[SISTEMA]: Conectando ao Banco Central...");
Thread.Sleep(1000);
Console.Write("[SISTEMA]: Calculando taxas");
```

✔ O sistema comunica suas ações ao usuário  
✔ Simula processamento real  
✔ Reduz incerteza e melhora a experiência de uso  

O uso de mensagens e animação com pontos (`...`) cria feedback visual contínuo, mostrando que o programa está ativo.

---

### ⚠️ 2. Prevenção de Erros

A prevenção de erros busca evitar que o usuário fique confuso ou que o sistema falhe sem explicação.

No projeto, foi implementado o bloco `try-catch`, responsável por capturar entradas inválidas:

```csharp
catch (Exception)
{
    Console.WriteLine("Entrada inválida! Use apenas números e vírgula para decimais.");
}
```

✔ Evita o encerramento inesperado do programa  
✔ Identifica erros de digitação do usuário  
✔ Apresenta mensagem clara e educativa  

Além disso, o uso de cores destaca visualmente o erro, facilitando a compreensão imediata.

---

### 🎨 3. Estética e Design Minimalista

Essa heurística defende interfaces simples, organizadas e com foco apenas nas informações essenciais.

Aplicação no código:

```csharp
Console.ForegroundColor = ConsoleColor.Green;
Console.WriteLine($"VALOR CONVERTIDO: $ {resultado:F2} (Dólares)");
```

✔ Interface limpa e objetiva  
✔ Destaque visual apenas para o resultado principal  
✔ Uso estratégico de cores para hierarquia da informação  

Linhas separadoras e cores ajudam o usuário a identificar rapidamente o resultado da conversão.

---

## 📌 Conclusão
Evidência do funcionamento completo do programa:
[Imagem do Programa Completo](https://github.com/manulaportee/una-ihcux-lista05/blob/main/Imagem%20do%20Programa%20Completo.png)

O sistema demonstra que princípios de UX podem ser aplicados mesmo em aplicações de console.  
As heurísticas utilizadas contribuem para:

- Melhor comunicação entre sistema e usuário
- Redução de erros de uso
- Interface mais clara e agradável

Assim, o projeto une **programação** e **usabilidade**, proporcionando uma experiência mais intuitiva e eficiente.

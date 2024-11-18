# Ranking
Calculadora de partidas Rankeadas

    // Função que calcula o saldo e o nível do jogador  
    function calcularRank(vitorias, derrotas) {  
    // Calculando o saldo de vitórias  
    const saldoVitorias = vitorias - derrotas;  
    let nivel;  
    // Determinando o nível baseado no número de vitórias
    if (vitorias < 10) {
        nivel = "Ferro";
    } else if (vitorias >= 11 && vitorias <= 20) {
        nivel = "Bronze";
    } else if (vitorias >= 21 && vitorias <= 50) {
        nivel = "Prata";
    } else if (vitorias >= 51 && vitorias <= 80) {
        nivel = "Ouro";
    } else if (vitorias >= 81 && vitorias <= 90) {
        nivel = "Diamante";
    } else if (vitorias >= 91 && vitorias <= 100) {
        nivel = "Lendário";
    } else if (vitorias >= 101) {
        nivel = "Imortal";
    }

    // Mensagem final
    console.log(`O Herói tem saldo de ${saldoVitorias} e está no nível ${nivel}.`);  
    }  
    
    // Exemplo de uso:  
    // Você pode alterar esses valores para testar  
    const vitorias = 55;  
    const derrotas = 20;  
    
    calcularRank(vitorias, derrotas);


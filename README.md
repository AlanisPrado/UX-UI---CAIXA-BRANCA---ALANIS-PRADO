# UX-UI---CAIXA-BRANCA---ALANIS-PRADO
#   NOTAÇÃO DE GRAFO DE FLUXO

1 -> Início do método  
2 -> Conectar ao banco  
3 -> Executar SQL  
4 -> if (rs.next())  
5 -> return true  
6 -> return false  
7 -> catch (erro)

# FLUXO:
1-> 2-> 3-> 4-> 5
1-> 2-> 3-> 4-> 6
1-> 2-> 3-> 7
1-> 2-> (erro direto)

# COMPLEXIDADE CICLOMATICA 

Fórmula: V(G) = E – N + 2  
E = 9, N = 7  
V(G) = 9 – 7 + 2 = 4
Complexidade Ciclomatica = 4


# CAMINHOS BASICOS

CAMINHO (1) = 1-2-3-4-5   // Quando login e senha esta correto
CAMINHO (2) = 1-2-3-4-6   // Quando  estão incorreto
CAMINHO (3) = 1-2-3-7     // Erro ao executar SQL
CAMINHO (4) = 1-2-7       // Quando a conexão com o banco falha antes de executar

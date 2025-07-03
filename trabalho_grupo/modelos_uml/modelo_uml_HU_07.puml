@startuml
' Versão simplificada do diagrama de classes

class SistemaMonitoramento {
}

class Sensor {
  - id: String
  - localizacao: String
  + getLeitura(): LeituraSensor
}

class LeituraSensor {
  - timestamp: DateTime
  - valor: Float
}

class GerenciadorDados {
  + coletar(): List<LeituraSensor>
  + filtrar(tipo: String, periodo: String): List<LeituraSensor>
}

class GerenciadorVisualizacao {
  + renderizarGrafico(leituras: List<LeituraSensor>): void
  + renderizarMapa(sensores: List<Sensor>): void
}

' Relacionamentos básicos
SistemaMonitoramento "1" *-- "1" GerenciadorDados
SistemaMonitoramento "1" *-- "1" GerenciadorVisualizacao

GerenciadorDados "1" o-- "*" Sensor
GerenciadorDados "1" o-- "*" LeituraSensor

GerenciadorVisualizacao ..> GerenciadorDados

@enduml

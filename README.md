# Documentação do Software ClassFace

## 1. Introdução

1.1 Visão Geral

O ClassFace é um sistema de chamada automática para salas de aula que utiliza reconhecimento facial para registrar a presença dos alunos. O objetivo é modernizar o controle de presença acadêmico, garantindo mais segurança, agilidade e transparência no processo. O sistema é composto por um aplicativo mobile integrado a dispositivos IoT e a um banco de dados baseado em Big Data.

1.2 Objetivo do Documento

Esta documentação detalha as especificações técnicas, requisitos, funcionalidades e arquitetura do sistema ClassFace, servindo como referência para desenvolvedores, administradores de sistema e demais stakeholders.

## 2. Tecnologias Utilizadas

O sistema ClassFace utiliza as seguintes tecnologias:

Linguagens: Python, JavaScript (React Native, Node.js)

Frameworks e Bibliotecas: OpenCV, TensorFlow, Express.js

Banco de Dados: PostgreSQL, Firebase (para sincronização em tempo real)

Serviços de Nuvem: AWS ou Google Cloud

Hardware: Câmeras IoT compatíveis com protocolo de transmissão em rede

Mobile: React Native para desenvolvimento do aplicativo

## 3. Arquitetura do Sistema

O ClassFace segue uma arquitetura baseada em microserviços e comunicação entre dispositivos IoT, mobile e servidores em nuvem.

3.1 Backend

Responsável pelo processamento das imagens capturadas pelas câmeras.

Utiliza Python com TensorFlow para reconhecimento facial.

API REST desenvolvida em Node.js e Express.js.

Banco de dados PostgreSQL para armazenamento dos registros de presença.

Firebase para sincronização de dados em tempo real entre dispositivos móveis e backend.

3.2 Frontend (Mobile)

Aplicativo mobile desenvolvido com React Native.

Permite que professores e alunos acompanhem os registros de presença.

Interface intuitiva para visualização de frequência e alertas de ausência.

3.3 Dispositivos IoT

Câmeras conectadas ao sistema capturam imagens e transmitem os dados para processamento.

Comunicação via MQTT ou HTTP com o backend.

## 4. Funcionalidades

4.1 Registro Automático de Presença

Captura imagens dos alunos e identifica suas presenças automaticamente.

4.2 Integração com Sistemas Acadêmicos

Sincroniza os registros de presença com os sistemas institucionais existentes.

4.3 Relatórios e Painel de Controle

Professores e gestores podem acessar históricos detalhados de presença por meio do aplicativo móvel.

Geração de gráficos e análises preditivas baseadas em Big Data.

4.4 Notificações e Alertas

O aplicativo mobile envia notificações automáticas para alunos, professores e responsáveis em caso de faltas frequentes.

## 5. Requisitos

5.1 Requisitos Funcionais

O sistema deve permitir o reconhecimento facial dos alunos.

O sistema deve armazenar e exibir históricos de presença.

O sistema deve possibilitar a integração com plataformas acadêmicas.

O aplicativo deve fornecer relatórios e notificações sobre a frequência dos alunos.

5.2 Requisitos Não Funcionais

Alta disponibilidade e escalabilidade.

Segurança dos dados com criptografia.

Suporte para múltiplas câmeras simultaneamente.

Sincronização em tempo real com dispositivos móveis.

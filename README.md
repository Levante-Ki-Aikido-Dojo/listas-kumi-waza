# Listas de kumi waza

Este proyecto contiene las listas de las técnicas de los exámenes de kyu (kumi waza) de ki aikido en formato JSON. Este formato de texto permite que puede gestionar por un sistema de control de versiones. Luego a base de estos documentos se puede convertir al formato ODS, lo cuál se puede abrir con un programa de hojas de cálculo.

## Preparación

Crear un Python virtual environment:

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt 
```

## Generar ODS

```bash
odsgenerator 1kyu.json 1kyu.ods
```

Recuerda de después de generar el ODS, remover manualmente el header y footer de la hoja.

## Generar JSON

```bash
odsparsator -k 1kyu.ods 1kyu.json
```

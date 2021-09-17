
def nucleoToDinucleo(rna):
  diNucleo = []
  for i in range(0,len(rna),2):
    if(len(rna)>i):
      diNucleo.append(rna[i]+rna[i+1])
    else:
      diNucleo.append(rna[i])
  return diNucleo

def comparador(seq1, seq2):
  diNucleo1 = nucleoToDinucleo(seq1)
  diNucleo2 = nucleoToDinucleo(seq2)
  resultado = {}
  tamanhoLista = None
  if len(diNucleo1)>=len(diNucleo2):
    tamanhoLista = len(diNucleo1)
  else:
    tamanhoLista = len(diNucleo2)

  for par in range(tamanhoLista-1):
    resultado[par]=[diNucleo1[par]==diNucleo2[par],diNucleo1[par],diNucleo2[par]]
  return resultado

seq1 = 'ATGACTGATCGATCGACTGACTGACCGCGCGCGCGATCGACTGACTGACTAGCTAGCATCGACTGACTGCGCGCGCGATCGATCAGCGACTAGCTAGCTACG'
seq2 = 'ATATGCGCGAATGCATCGATGCTAGCTGACTGATCGATGCATGCCGCGCGCGCGCGACGACTGATCGCGCGCGATCGATCGATCGGCGCGCATCGACGATGC'
result = comparador(seq1,seq2)

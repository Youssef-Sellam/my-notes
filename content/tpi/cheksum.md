per fare il cheksum si deve prima scaricare [il file](https://download.fedoraproject.org/pub/fedora/linux/releases/40/Server/x86_64/iso/Fedora-Server-40-1.14-x86_64-CHECKSUM)  poi  devi controllare 
quello che di dice Fedora !

1. **Scarica il file CHECKSUM**: Scarica il file di cheksum dal link che hai fornito.
![[Pasted image 20241028111111.png]]
    
2. **Scarica l'immagine ISO**: Scarica l'immagine ISO che vuoi verificare. Assicurati che il nome del file ISO corrisponda a quello nel file di cheksum.
    
3. **Verifica il cheksum**:
    
    - Apri un terminale (cmd su Windows, terminale su MacOS o Linux).
        
    - Naviga nella directory dove hai scaricato il file ISO e il file CHECKSUM. Puoi usare il comando `cd` seguito dal percorso della directory.
        
4. **Esegui il comando per verificare il cheksum**:
    
    - Su **Windows**, utilizza `CertUtil`:
        
        cmd
        
        ```
        certutil -hashfile <nome-file-ISO> SHA256
        ```
        
        Confronta l'output di questo comando con il valore nel file CHECKSUM.
        
    - Su **MacOS** e **Linux**, utilizza `sha256sum`:
        
        bash
        
        ```
        sha256sum <nome-file-ISO>
        ```
        
        Confronta l'output di questo comando con il valore nel file CHECKSUM.
        

Ecco un esempio di come dovrebbe apparire:

bash

```
$ sha256sum Fedora-Server-40-1.14-x86_64.iso
<checksum-calculato>  Fedora-Server-40-1.14-x86_64.iso
```

Confronta `<checksum-calculato>` con il valore nel file CHECKSUM scaricato.

Se i due valori corrispondono, significa che il file scaricato è integro e non è stato alterato.
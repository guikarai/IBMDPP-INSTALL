## Download the IBM Data Privacy Passports Appliance

## Preparing the Installation Manager client machine

## Set up the Data Privacy Passports Manager utility

### 1. Go to the client machine.

### 2. Go to the directory with all the downloaded files.

:computer: We defined earlier /dpp. So issue the following command:
```
cd /dpp
```

### 3. Create a hpvs-vars.json file from one of the templates.

:computer: As example, you can reuse and copy the hpvs-vars-small.json file. Please issue the following command:
```
cp hpvs-vars-small.json hpvs-vars.json
```

### 4. Test the dpp-manager. 

:computer: Please, issue the following command.
```
python3 dpp-manager.py help
usage: python dpp-manager.py <option> [container]
options:
    help:                list help options
    token:               generate or update an HPVS authentication token
    tag [tag-name]:      update the tag for all containers
    install:             generate a token, then load and start DPP containers
    containers:          list information about containers on HPVS
    clean:               delete all containers and prune all unused images
    prune:               prune DPP images
    load [tar-file]:     load DPP images to HPVS from tar.gz file. Specify a file name to load a single image
    create [container]:  create and start DPP containers. Specify container name to create a single container
    update [container]:  update DPP containers. Specify container name to create a single container
    delete [container]:  delete DPP containers. Specify container name to delete a single container
    start [container]:   start DPP containers. Specify container name to start a single container
    stop [container]:    stop DPP containers. Specify container name to stop a single container
    restart [container]: restart DPP containers. Specify container name to restart a single container
    network create:      create DPP network
    network inspect:     retrieve DPP network details
    network delete:      delete DPP network
    quotagroups create:  create quotagroups
    quotagroups inspect: retrieve quotagroup details
    quotagroups delete:  delete quotagroups
```

###5. Ready for next steps?

It it works, continue to next step. If not, installany additional pre-requisites.


## Configure the Data Privacy Passports Manager utility JSON

Update the hypvs-vars.json file according to your environment (see doc)

Add SSL Enablement And LDAP Truststore Password Envars.  

This is needed only for TLS but doesn’t hurt to put it in now to prepare for TLS)

* "ZSTG_LDAP_TRUSTSTORE_PASS": "",
* "LDAP_SSL_ENABLED": "true",

## 

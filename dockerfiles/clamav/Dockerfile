FROM $org.opensuse
#FROM amacdexp/opensuseleap151:latest


#Setup files for clamav
RUN mkdir /home/vflow/data


#Switch back too root for install [SAP DI Prereq]
USER root:root

RUN zypper install -y clamav 

#Loads Virus database
RUN freshclam 

# permission juggling (not working in DI...)
#RUN chown -R 1972:1972 /var/run/clamav/ #&& \
#    chmod 750 /var/run/clamav && \
#    chown -R 1972:1972 /var/lib/clamav/ 



# Switchback to VFLOW user [SAP DI Prereq]
USER 1972:1972

#Boto3 used to access S3
RUN python3 -m pip --no-cache-dir install boto3 --user


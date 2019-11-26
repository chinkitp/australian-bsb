FROM postgres:10.1

ENV BASE_URL 'ftp://bsb.hostedftp.com/~auspaynetftp/bsb/'
ENV KEY_ABBREVIATION_FILE 'KEY TO ABBREVIATIONS AND BSB NUMBERS (Sep 2019).csv'
ENV BASE_DATA_FILE 'BSBDirectorySep19-282.csv'
ENV UPDATE_FILE 'BSB Directory Update 03Sept19-01Oct19.csv'

ADD setup /
ADD docker-entrypoint-initdb.d /docker-entrypoint-initdb.d
ADD SqlScripts /SqlScripts
RUN /setup

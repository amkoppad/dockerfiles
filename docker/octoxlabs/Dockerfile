# Last modified: 2024-03-04T16:36:38.542752+00:00
FROM demisto/python3:3.10.13.89009

COPY requirements.txt .

RUN apk --update add --no-cache --virtual .build-dependencies python3-dev build-base wget git \
  && pip install --no-cache-dir -r requirements.txt \
  && apk del .build-dependencies

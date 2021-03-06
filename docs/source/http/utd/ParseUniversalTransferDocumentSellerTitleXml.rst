ParseUniversalTransferDocumentSellerTitleXml
============================================

Имя ресурса: **/ParseUniversalTransferDocumentSellerTitleXml**

HTTP метод: **POST**

В теле запроса должен содержаться XML-файл в формате титула продавца УПД.

Файл титула продавца УПД изготавливается в соответствии с :download:`XML-схемой <../../xsd/ON_SCHFDOPPR_1_995_01_05_01_02.xsd>`, которому должны удовлетворять XML-счета-фактуры, согласно приказу ФНС.

В теле ответа содержится сериализованная структура :doc:`../../proto/utd/UniversalTransferDocumentSellerTitleInfo`, построенная на основании данных запроса.

Возможные HTTP-коды возврата:

-  200 (OK) - операция успешно завершена;

-  400 (Bad Request) - данные в запросе имеют неверный формат или отсутствуют обязательные параметры;

-  405 (Method not allowed) - используется неподходящий HTTP-метод;

-  500 (Internal server error) - при обработке запроса возникла непредвиденная ошибка.

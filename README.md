# hse_hw2_chip

Я взял клеточную линию PC-3, гистоновая метка H3K27me3 (https://www.encodeproject.org/experiments/ENCSR881TWJ/).

Реплика 1 - ENCFF281ZEA; Реплика 2 - ENCFF299BLB; Контроль - ENCFF829PCB.

# FastQC

## ENCFF281ZEA (реплика 1)

![image](https://user-images.githubusercontent.com/93254228/156644494-a335b367-b5d8-489d-8e3d-1e8b96b7ea9e.png)

![image](https://user-images.githubusercontent.com/93254228/156644533-1f352d80-8aa4-476d-93c8-9f4c1119b759.png)

![image](https://user-images.githubusercontent.com/93254228/156644586-52012ee6-6cdc-423a-b0f4-96e733618d4d.png)
 
 Как видно из графика Per tile sequence quality, требуется провести подрезание для данного чтения (используем trimmomatic).
 
 Что имеем на выходе:
 
 ![image](https://user-images.githubusercontent.com/93254228/156645382-9edbf652-1b17-4696-9523-4df71ae52a47.png)

![image](https://user-images.githubusercontent.com/93254228/156645453-8f5670c1-e7a5-457f-8ae7-cb1e915885a9.png)

![image](https://user-images.githubusercontent.com/93254228/156645499-fb69938c-6d65-422e-a1d3-2d1e91186889.png)

Как видно, ситуация улучшилась как с Per tile sequence quality, так и с Per base sequence quality.

## ENCFF299BLB (реплика 2)

![image](https://user-images.githubusercontent.com/93254228/156645905-6507480a-1129-4545-b46f-926c9bb11d49.png)

![image](https://user-images.githubusercontent.com/93254228/156645962-607bbd27-311e-471b-b653-0eea8b632cff.png)

![image](https://user-images.githubusercontent.com/93254228/156646000-f50236e7-5ea7-4dd8-998d-97ab00518882.png)

Здесь подрезания не потребовались.

## ENCFF829PCB (контрольный образец)

![image](https://user-images.githubusercontent.com/93254228/156647135-27d2e93c-2213-4d94-a9b1-49d593b627c9.png)

![image](https://user-images.githubusercontent.com/93254228/156647213-f780adf2-c0b8-4aaa-8a89-98f8cbd73b9a.png)

![image](https://user-images.githubusercontent.com/93254228/156647248-4db930fe-5740-40dc-8b5a-3da11c9f0d50.png)

Видно, что, как и в случае первой реплики, нужно использовать trimmomatic для подрезания.

Итог:

![image](https://user-images.githubusercontent.com/93254228/156647373-a77ea302-a42d-4f48-b807-3042d8b3f6a6.png)

![image](https://user-images.githubusercontent.com/93254228/156647399-d97a88d3-a646-4421-99d5-9bde19dcf7cf.png)

![image](https://user-images.githubusercontent.com/93254228/156647450-e41a3c70-44e3-410a-92a6-a7922216e00b.png)

Ситуация очень похоже на ту, что наблюдалась при подрезании первой реплики.

# Bowtie

Таблица с результатами анализа bowtie:

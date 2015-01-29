float* mapping(float prvImg[], float desireH1[]){
	float newImg[256];
	int indB = 0;
	re(indA, 0, 256){
		if (prvImg[indA] <= desireH1[indB] && !indB)
			newImg[indA] = indB;
		else if (prvImg[indA] > desireH1[indB])
		{
			indB++;
			indA--;
		}
		else if (indB){
			//spec[indA]=indB-(a[indA] - b[indB - 1] < a[indA] - b[indB]);
			if (abs(prvImg[indA] - desireH1[indB - 1]) >= abs(prvImg[indA] - desireH1[indB]))
				newImg[indA] = indB;
			else
				newImg[indA] = indB - 1;
		}
	}
	return newImg;
}

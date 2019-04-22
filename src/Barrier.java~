//package BarrierS;
import java.util.concurrent.Semaphore;

public class Barrier {
	
	// add missing variables
	int n;
	int incrementer;
	Semaphore semaphore;
	Semaphore semaphore2;
	Semaphore semaphore3;
	Semaphore semaphore4;
	
	Barrier(int n) {
		// complete this constructor
		this.semaphore = new Semaphore(n+1);
		this.semaphore2 = new Semaphore(n);
		this.semaphore3 = new Semaphore(n+1);
		this.semaphore4 = new Semaphore(n);
		this.n=n;
	}
	
	public void b_wait() throws InterruptedException{
		// this is the only additional method you will need to complete
		semaphore.acquire();
		incrementer++;
		semaphore.release();
		
		while(incrementer < n){
			semaphore2.release();
			}
		semaphore2.acquire();
		semaphore2.release();
	}

}

import { Component, OnInit } from '@angular/core';
import { HttpClient } from '@angular/common/http';
import { ApiService } from 'src/app/shared/services/api.service';

@Component({
      selector: 'app-testing',
      templateUrl: './testing.component.html',
      styleUrls: ['./testing.component.scss']
    })
    export class TestingComponent implements OnInit {
      
      

                screenData1: any;
                    verticalBarChartOptions1: any = {
                        plugins: {
                            legend: {
                                labels: {
                                    color: '#495057'
                                }
                            }
                        },
                        scales: {
                            x: {
                                ticks: {
                                    color: '#495057'
                                },
                                grid: {
                                    color: '#ebedef'
                                }
                            },
                            y: {
                                ticks: {
                                    color: '#495057'
                                },
                                grid: {
                                    color: '#ebedef'
                                }
                            }
                        }
                    }
                
constructor(private http: HttpClient, private api: ApiService) { }
 ngOnInit(): void {
 this.getData()
} 
getData(): void {
  this.getData1();
}

getData1(): void {
    this.screenData1 = {"labels":["January","February","March","April","May","June","July"],"datasets":[{"label":"My First dataset","backgroundColor":"#42A5F5","data":[65,59,80,81,56,55,40]},{"label":"My Second dataset","backgroundColor":"#FFA726","data":[28,48,40,19,86,27,90]}]}
 }


}

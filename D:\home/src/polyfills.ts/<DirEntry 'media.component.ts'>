import { Component, OnInit } from '@angular/core';
import { HttpClient } from '@angular/common/http';
import { ApiService } from 'src/app/shared/services/api.service';

@Component({
      selector: 'app-media',
      templateUrl: './media.component.html',
      styleUrls: ['./media.component.scss']
    })
    export class MediaComponent implements OnInit {
      
      
screenData1!: string;
 latitude: any;
 longitude: any;
 zoom: any;

constructor(private http: HttpClient, private api: ApiService) { }
 ngOnInit(): void {
 this.getData()
} 
getData(): void {
  this.getData1();
}

getData1(): void {
    this.screenData1 = [{"latitude":"16.9891","longitude":"82.2475","zoom":"12","apiKey":""}]
 }


}

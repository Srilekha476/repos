import { Component, OnInit } from '@angular/core';
import { HttpClient } from '@angular/common/http';
import { ApiService } from 'src/app/shared/services/api.service';

@Component({
      selector: 'app-media',
      templateUrl: './media.component.html',
      styleUrls: ['./media.component.scss']
    })
    export class MediaComponent implements OnInit {
      
      
 showSuggestions1: boolean = false;
 screenData1 = new FormControl(null, [Validators.required, Validators.pattern('^[^\s@]+@[^\s@]+\.[^\s@]{2,4}$')]);
screenData2: any;

screenData3: any[] = [];
 bindingValue3: '';

screenData4: any[] = [];
 bindingValue4: any;

singledate: Date = new Date();

                minDate = new Date();

                maxDate=  new Date();
 
screenData6: any[] = [];
 bindingValue6: any;

multipledates: Date;
                minDate = new Date();

                maxDate=  new Date();
 
screenData8: any[] = [];
 bindingValue8: '';

constructor(private http: HttpClient, private api: ApiService) { }
 ngOnInit(): void {
 this.getData()
} 
getData(): void {
  this.getData1();
  this.getData2();
  this.getData3();
  this.getData4();
  this.getData5();
  this.getData6();
  this.getData7();
  this.getData8();
}

getData1(): void {
    this.screenData1 = ["shankar.a@arkatiss.com"]
 }

getData2(): void {
    this.screenData2 = ["Arkatiss@1234"]
 }

getData3(): void {
    this.screenData3 = []
 }

getData4(): void {
    this.screenData4 = [null]
 }

getData5(): void {
    this.screenData5 = undefined
 }

getData6(): void {
    this.screenData6 = []
 }

getData7(): void {
    this.screenData7 = undefined
 }

getData8(): void {
    this.screenData8 = []
 }


}
